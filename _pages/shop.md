---
layout: default
title: Shop
header_type: hero
header_img: /assets/images/IMG_0190.webp
permalink: /shop/
active_shopify_product_ids:
  - "8317324296383" # the wave
  - "8317321380031" # the peach
  - "8317313024191" # scorched arbutus
  - "8316215558335" # pommele sapele
  - "8317331341503" # credit card contoured
  - "8317331767487" # credit card straight
---

<style>
h1, h2, h3, h4, h5, h6 {
  color: var(--primary);
}

.shop-intro {
  font-size: 1.2rem;
  line-height: 1.6;
  text-align: center;
  max-width: 800px;
  margin: 2rem auto 3rem;
  color: #333;
}

.shopify-products-container {
  max-width: 1200px;
  margin: 2rem auto;
  padding: 0 1rem;
}

.shopify-product-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 2rem 1.25rem;
}

.shopify-product-item {
  min-width: 0;
}

.section-title {
  margin: 2rem 0 1rem;
  font-size: 1.8rem;
  text-align: center;
}

.section-content {
  max-width: 800px;
  margin: 0 auto 2rem;
  line-height: 1.6;
  color: #444;
}

@media (max-width: 768px) {
  .shop-intro {
    font-size: 1rem;
    padding: 0 1rem;
  }
}

/* Target the image wrapper inside the Shopify Modal */
.shopify-buy-modal-wrapper .shopify-buy__product-img-wrapper {
    max-width: 600px !important; /* Increase this number as needed */
    width: 100% !important;
}
</style>

## Shop Gatorface Woodworking
{: .section-title}

Browse our collection of handcrafted woodworking pieces. Each item is carefully made with sustainable practices and traditional techniques in our Nanaimo workshop.
{: .shop-intro}

<div class="shopify-products-container">
  <div id="shopify-product-list" class="shopify-product-list"></div>
</div>

<script type="text/javascript">
/*<![CDATA[*/
(function () {
  var scriptURL = 'https://sdks.shopifycdn.com/buy-button/latest/buy-button-storefront.min.js';
  if (window.ShopifyBuy) {
    if (window.ShopifyBuy.UI) {
      ShopifyBuyInit();
    } else {
      loadScript();
    }
  } else {
    loadScript();
  }

  function loadScript() {
    var script = document.createElement('script');
    script.async = true;
    script.src = scriptURL;
    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(script);
    script.onload = ShopifyBuyInit;
  }

  function ShopifyBuyInit() {
    var client = ShopifyBuy.buildClient({
      domain: '81w3df-wg.myshopify.com',
      storefrontAccessToken: '153a66932e4f9828338077058a0db2ed',
    });

    ShopifyBuy.UI.onReady(client).then(function (ui) {
      var productIds = [
        {% for product_id in page.active_shopify_product_ids %}
          '{{ product_id }}'{% unless forloop.last %},{% endunless %}
        {% endfor %}
      ];

      if (productIds.length === 0) {
        return;
      }

      var productListNode = document.getElementById('shopify-product-list');

      productIds.forEach(function (productId) {
        var productNode = document.createElement('div');
        productNode.id = 'shopify-product-' + productId;
        productNode.className = 'shopify-product-item';
        productListNode.appendChild(productNode);

        ui.createComponent('product', {
          id: productId,
          node: productNode,
          moneyFormat: '%24%7B%7Bamount%7D%7D',
          options: {
            "product": {
              "styles": {
                "product": {
                  "max-width": "100%",
                  "margin-left": "0px",
                  "margin-bottom": "0px",
                  "width": "100%"
                },
                                "button": {
        ":hover": {
          "background-color": "#a0bd30"
        },
        "background-color": "#b2d235",
        ":focus": {
          "background-color": "#a0bd30"
        }
                                }
              },
              "buttonDestination": "modal",
              "contents": {
                "img": true,
                "imgWithCarousel": false,
                "title": true,
                "price": true,
                "description": false,
                "button": true,
                "quantity": false
              },
              "text": {
                "button": "View details"
              }
            },
            "modalProduct": {
              "layout": "horizontal",
              "width": "1200px",
              "contents": {
                "img": false,
                "imgWithCarousel": true,
                "description": true,
                "button": false,
                "buttonWithQuantity": true
              },
              "styles": {
                "product": {
      "@media (min-width: 601px)": {
        "max-width": "100%",
        "margin-left": "0px"
      },
       "img": {
      "width": "100%",
      "height": "auto",
      "object-fit": "contain"
    }
    },

    // This targets the main image inside the Shopify carousel
    "carouselProduct": {
        "height": "600px", // Forces the container to be taller
        "margin-bottom": "20px"
    },
    "img": {
      "width": "100% !important",
      "height": "auto !important",
      "object-fit": "contain",
      "cursor": "zoom-in",
      "transition": "transform 0.3s ease-in-out",
      ":hover": {
        "transform": "scale(1.4)" // The zoom effect
      }
    },
    "imgWrapper": {
        "overflow": "hidden !important" // Clips the zoom so it doesn't overlap text
    }
              },
              "text": {
                "button": "Add to cart"
              }
            },
            "option": {},
            "cart": {
              "text": {
                "total": "Subtotal",
                "button": "Checkout"
              }
            },
            "toggle": {}
          },
        });
      });
    });
  }
})();
/*]]>*/
</script>


---

## Custom Orders
{: .section-title}

Looking for something specific? We also take custom orders for furniture and home goods tailored to your space and style. Each custom piece is a collaboration designed to meet your unique needs.
{: .section-content}

[Contact Me About Custom Work](/contact/){: .cta-button .btn .btn-primary .d-block .mx-auto style="width: fit-content; margin: 2rem auto; padding: 1rem 2rem; background-color: var(--secondary); color: var(--secondary-inverse) !important; text-decoration: none; border-radius: 4px; font-weight: bold; transition: background-color 0.3s ease;"}

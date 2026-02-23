---
layout: default
title: Order Confirmation
header_type: hero
header_img: /assets/images/IMG_0190.webp
permalink: /order-confirmation/
---

Note: Shopify handles order confirmations automatically. This page is shown if you redirect here after checkout.

<style>
h1, h2, h3, h4, h5, h6 {
  color: var(--primary);
}

.confirmation-container {
  max-width: 800px;
  margin: 3rem auto;
  padding: 0 1rem;
  text-align: center;
}

.confirmation-icon {
  font-size: 4rem;
  color: var(--secondary);
  margin-bottom: 1.5rem;
}

.confirmation-title {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  color: var(--primary);
}

.confirmation-message {
  font-size: 1.2rem;
  line-height: 1.8;
  color: #333;
  margin-bottom: 2rem;
}

.info-box {
  background-color: #f7f6f5;
  border-left: 4px solid var(--secondary);
  padding: 1.5rem;
  margin: 2rem 0;
  text-align: left;
  border-radius: 4px;
}

.info-box h3 {
  margin-top: 0;
  margin-bottom: 1rem;
  color: var(--primary);
  font-size: 1.3rem;
}

.info-box p {
  margin-bottom: 0.75rem;
  color: #444;
  line-height: 1.6;
}

.info-box p:last-child {
  margin-bottom: 0;
}

.contact-link {
  display: inline-block;
  margin-top: 2rem;
  padding: 1rem 2rem;
  background-color: var(--secondary);
  color: var(--secondary-inverse) !important;
  text-decoration: none;
  border-radius: 4px;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.contact-link:hover {
  background-color: var(--secondary-dark);
  text-decoration: none;
  color: var(--secondary-inverse) !important;
}

@media (max-width: 768px) {
  .confirmation-title {
    font-size: 2rem;
  }
  
  .confirmation-message {
    font-size: 1rem;
  }
  
  .confirmation-container {
    margin: 2rem auto;
  }
}
</style>

<div class="confirmation-container">
  <div class="confirmation-icon">
    <i class="fas fa-check-circle"></i>
  </div>
  
  <h1 class="confirmation-title">Thank You for Your Order!</h1>
  
  <p class="confirmation-message">
    Your order has been successfully placed. We're excited to get your handcrafted piece ready for you!
  </p>
  
  <div class="info-box">
    <h3><i class="fas fa-shipping-fast" style="margin-right: 0.5rem;"></i> Shipping Information</h3>
    <p><strong>Your order should ship within 3-5 business days.</strong> You'll receive a shipping confirmation email with tracking information once your item is on its way.</p>
    <p>Each piece is carefully crafted by hand in our Nanaimo workshop, so please allow a few days for us to ensure everything is perfect before shipping.</p>
  </div>
  
  <div class="info-box">
    <h3><i class="fas fa-question-circle" style="margin-right: 0.5rem;"></i> Questions?</h3>
    <p>If you have any questions about your order or need to make changes, please don't hesitate to reach out. We're here to help!</p>
    <p><strong>Email:</strong> <a href="mailto:paul@gatorfacewoodworking.ca">paul@gatorfacewoodworking.ca</a></p>
    <p><strong>Phone:</strong> <a href="tel:778-268-1146">778-268-1146</a></p>
  </div>
  
  <a href="/contact/" class="contact-link">
    <i class="fas fa-envelope" style="margin-right: 0.5rem;"></i>Contact Us
  </a>
  
  <div style="margin-top: 3rem;">
    <a href="/shop/" style="color: var(--primary); text-decoration: underline;">Continue Shopping</a>
  </div>
</div>

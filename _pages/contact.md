---
layout: default
title: Contact
header_type: hero
header_img: /assets/images/IMG_0190.jpg
permalink: /contact/
---

<div class="container-fluid">
  <div class="intro-section">
    <h1>Let's Talk About Your Project</h1>
    <p>Got an idea for a custom piece? Or maybe you just want to chat about what's possible? I'm all ears!</p>
  </div>

  <div class="contact-page-container">
    <div class="contact-content">
      <h2>Drop Us a Line</h2>
      <div class="contact-info">
        <p><strong>Email:</strong> <a href="mailto:paul@gatorfacewoodworking.ca">paul@gatorfacewoodworking.ca</a></p>
        <p><strong>Phone:</strong> <a href="tel:778-268-1146">778-268-1146</a></p>
        <p><strong>Workshop open by appointment only</strong></p>
      </div>
    </div>

    <div class="map-container">
      <div class="map-sticky">
        <iframe 
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2605.72244441687!2d-124.02183518693799!3d49.224790674731246!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x548899c21d4967d1%3A0x8dfa27c40d9aaad9!2sGatorface%20Woodworking!5e0!3m2!1sen!2sca!4v1739991490075!5m2!1sen!2sca" 
          width="100%" 
          height="450" 
          style="border:0;" 
          allowfullscreen="" 
          loading="lazy" 
          referrerpolicy="no-referrer-when-downgrade">
        </iframe>
      </div>
    </div>
  </div>

  <div class="form-section">
    <h2>Tell Us What You're Dreaming Up</h2>

    <div class="contact-form-container">
      <form action="https://formspree.io/f/xeoevpvb" method="POST" class="contact-form">
        <div class="form-group">
          <label for="name">What's your name?</label>
          <input type="text" name="name" id="name" required class="form-control" placeholder="Your name">
        </div>
        
        <div class="form-group">
          <label for="email">How can we reach you?</label>
          <input type="email" name="email" id="email" required class="form-control" placeholder="Your email">
        </div>
        
        <div class="form-group">
          <label for="message">Tell us more about what you have in mind:</label>
          <textarea name="message" id="message" rows="5" required class="form-control" placeholder="Share your ideas, questions, or just say hi!"></textarea>
        </div>
        
        <button type="submit" class="btn btn-primary">Send It Our Way →</button>
      </form>
    </div>
  </div>
</div>

<style>
.intro-section {
  text-align: center;
  max-width: 800px;
  margin: 0 auto 4rem;
  padding: 2rem 1rem;
}

.intro-section h1 {
  margin-bottom: 1.5rem;
  color: var(--primary);
}

.intro-section p {
  font-size: 1.2rem;
  line-height: 1.6;
  color: #666;
}

.contact-page-container {
  display: grid;
  grid-template-columns: minmax(auto, 800px) minmax(400px, 500px);
  gap: 3rem;
  margin: 0 auto 4rem;
  align-items: center;
  min-height: 450px;
}

.contact-content {
  padding-right: 0;
  max-width: 800px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
}

.contact-content h2 {
  margin-bottom: 1.5rem;
  color: var(--primary);
}

.contact-info {
  margin: 1rem 0;
  padding: 1.25rem;
  background-color: rgba(91, 81, 60, 0.05);
  border-radius: 8px;
  text-align: left;
}

.contact-info p {
  margin: 0.5rem 0;
  font-size: 1.1rem;
  word-break: break-all;
}

.contact-info a {
  color: var(--primary);
  text-decoration: none;
  transition: opacity 0.2s ease;
  word-break: normal;
}

.contact-info a:hover {
  opacity: 0.8;
}

.form-section {
  max-width: 800px;
  margin: 0 auto;
  padding: 3rem 0;
  text-align: center;
}

.form-section h2 {
  margin-bottom: 2rem;
  color: var(--primary);
}

.contact-form-container {
  margin: 2rem auto;
  padding: 2.5rem;
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  text-align: left;
}

.form-group {
  margin-bottom: 1.5rem;
}

.form-control {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid #ddd;
  border-radius: 6px;
  transition: border-color 0.2s ease;
}

.form-control:focus {
  border-color: var(--primary);
  outline: none;
  box-shadow: 0 0 0 2px rgba(91, 81, 60, 0.1);
}

.btn-primary {
  background-color: var(--secondary);
  color: var(--secondary-inverse);
  padding: 0.75rem 1.5rem;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.btn-primary:hover {
  opacity: 1;
  background-color: var(--secondary-dark);
  color: var(--secondary-inverse);
}

.map-container {
  position: relative;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.map-sticky {
  position: sticky;
  top: 2rem;
}

.map-sticky iframe {
  border-radius: 8px;
}

textarea.form-control {
  resize: vertical;
  min-height: 120px;
}

label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: bold;
  color: var(--primary);
}

@media (max-width: 1200px) {
  .contact-page-container {
    grid-template-columns: minmax(auto, 600px) 400px;
    gap: 2rem;
  }
  
  .contact-form-container {
    padding: 2rem;
  }
}

@media (max-width: 992px) {
  .intro-section {
    margin-bottom: 3rem;
  }

  .contact-page-container {
    grid-template-columns: 1fr;
    max-width: 800px;
    min-height: auto;
  }
  
  .contact-content {
    padding-right: 0;
    margin-bottom: 2rem;
  }
  
  .contact-info {
    margin: 1rem 0;
  }
  
  .map-sticky {
    position: static;
  }

  .map-container {
    margin-top: 2rem;
  }
  
  .form-section {
    padding: 2rem 1rem;
  }
}
</style> 
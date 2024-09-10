---
title: "Contact"
permalink: /contact/
layout: single
---

<div class="contact-container">
  <div class="contact-info">
    <h2>Contact Information</h2>
    <p>Email: {{ site.email }}</p>
    <p>LinkedIn: <a href="{{ site.linkedin_username }}">{{ site.linkedin_username }}</a></p>
    <p>Instagram: <a href="{{ site.instagram_username }}">{{ site.instagram_username }}</a></p>
    <p>Location: [Your Location]</p>
    [Insert small map here]
  </div>
  
  <div class="contact-form">
    <h2>Get in Touch</h2>
    <form action="https://formspree.io/f/your-form-id" method="POST">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>
      
      <label for="email">Email:</label>
      <input type="email" id="email" name="_replyto" required>
      
      <label for="subject">Subject:</label>
      <input type="text" id="subject" name="subject" required>
      
      <label for="message">Message:</label>
      <textarea id="message" name="message" required></textarea>
      
      <button type="submit">Send</button>
    </form>
  </div>
</div>
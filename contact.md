---
layout: default
title: Contact The Codedhans
---

# Get In Touch
Have a question about a tutorial or a project proposal? Drop a message below.

<div class="contact-form-container">
  <form action="https://formspree.io/f/codedspace1@gmail.com" method="POST">
    
    <label>Your Name:</label>
    <input type="text" name="name" required placeholder="John Doe">

    <label>Your Email:</label>
    <input type="email" name="_replyto" required placeholder="name@example.com">

    <label>Message:</label>
    <textarea name="message" rows="5" required placeholder="How can I help you?"></textarea>

    <input type="text" name="_gotcha" style="display:none">

    <button type="submit" class="btn-tutorial" style="width: 100%; border: none; cursor: pointer;">
        Send Message
    </button>
  </form>
</div>

<style>
  .contact-form-container {
    background: var(--white);
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    margin-top: 20px;
  }
  label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
    color: var(--navy);
  }
  input, textarea {
    width: 100%;
    padding: 12px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box; /* Crucial for mobile scaling */
    font-family: inherit;
  }
  input:focus, textarea:focus {
    border-color: var(--peru);
    outline: none;
  }
</style>

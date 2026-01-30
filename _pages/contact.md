---
layout: page
title: contact
permalink: /contact/
description: Get in touch with MIRAI VISION LAB
nav: true
nav_order: 7
---

<style>
.contact-page {
  max-width: 1200px;
  margin: 0 auto;
}

.contact-intro {
  text-align: center;
  margin: 2rem 0 4rem 0;
}

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3rem;
  margin: 3rem 0;
}

.contact-info-section {
  background: #fff;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.contact-form-section {
  background: #fff;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.contact-item {
  display: flex;
  align-items: flex-start;
  margin: 1.5rem 0;
  padding: 1rem;
  border-left: 4px solid #667eea;
  background: #f8f9fa;
  border-radius: 8px;
}

.contact-icon {
  font-size: 1.5rem;
  margin-right: 1rem;
  color: #667eea;
  min-width: 30px;
}

.contact-details h3 {
  margin: 0 0 0.5rem 0;
  font-size: 1.1rem;
  color: #2c3e50;
}

.contact-details p {
  margin: 0;
  color: #555;
  line-height: 1.6;
}

.contact-details a {
  color: #667eea;
  text-decoration: none;
}

.contact-details a:hover {
  text-decoration: underline;
}

.form-group {
  margin-bottom: 1.5rem;
}

.form-group label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: 600;
  color: #2c3e50;
}

.form-group input,
.form-group textarea,
.form-group select {
  width: 100%;
  padding: 0.75rem;
  border: 2px solid #e0e0e0;
  border-radius: 8px;
  font-size: 1rem;
  transition: border-color 0.3s ease;
}

.form-group input:focus,
.form-group textarea:focus,
.form-group select:focus {
  outline: none;
  border-color: #667eea;
}

.form-group textarea {
  min-height: 150px;
  resize: vertical;
}

.submit-btn {
  width: 100%;
  padding: 1rem;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  border: none;
  border-radius: 8px;
  font-size: 1.1rem;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.submit-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(102, 126, 234, 0.4);
}

.map-container {
  margin: 4rem 0;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.map-container iframe {
  width: 100%;
  height: 450px;
  border: none;
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin: 3rem 0;
  flex-wrap: wrap;
}

.social-link {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background: #667eea;
  color: white;
  font-size: 1.5rem;
  text-decoration: none;
  transition: transform 0.3s ease, background 0.3s ease;
}

.social-link:hover {
  transform: scale(1.1);
  background: #764ba2;
}

.directions-section {
  background: #f8f9fa;
  padding: 2rem;
  border-radius: 12px;
  margin: 3rem 0;
}

.directions-section h3 {
  margin: 0 0 1rem 0;
  color: #2c3e50;
}

.directions-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.directions-list li {
  padding: 0.75rem 0;
  border-bottom: 1px solid #e0e0e0;
  color: #555;
}

.directions-list li:last-child {
  border-bottom: none;
}

.directions-list li strong {
  color: #2c3e50;
  margin-right: 0.5rem;
}

@media (max-width: 768px) {
  .contact-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
  }
}
</style>

<div class="contact-page">
  <div class="contact-intro">
    <h1>Contact Us</h1>
    <p style="font-size: 1.2rem; color: #555; max-width: 800px; margin: 1rem auto;">
      We'd love to hear from you! Whether you're interested in research collaboration, 
      joining our team, or just want to learn more about our work, get in touch.
    </p>
  </div>

  <div class="contact-grid">
    <div class="contact-info-section">
      <h2 style="margin-top: 0;">Contact Information</h2>
      
      <div class="contact-item">
        <div class="contact-icon">📍</div>
        <div class="contact-details">
          <h3>Address</h3>
          <p>
            MIRAI VISION LAB<br>
            Building XYZ, Room 123<br>
            Department of Computer Science<br>
            University Name<br>
            City, State - 000000<br>
            Country
          </p>
        </div>
      </div>

      <div class="contact-item">
        <div class="contact-icon">📧</div>
        <div class="contact-details">
          <h3>Email</h3>
          <p>
            General Inquiries: <a href="mailto:info@miraivision.lab">info@miraivision.lab</a><br>
            Lab Director: <a href="mailto:director@miraivision.lab">director@miraivision.lab</a><br>
            Collaborations: <a href="mailto:collab@miraivision.lab">collab@miraivision.lab</a>
          </p>
        </div>
      </div>

      <div class="contact-item">
        <div class="contact-icon">📞</div>
        <div class="contact-details">
          <h3>Phone</h3>
          <p>
            Office: +1 (123) 456-7890<br>
            Lab: +1 (123) 456-7891<br>
            Fax: +1 (123) 456-7892
          </p>
        </div>
      </div>

      <div class="contact-item">
        <div class="contact-icon">🕒</div>
        <div class="contact-details">
          <h3>Office Hours</h3>
          <p>
            Monday - Friday: 9:00 AM - 5:00 PM<br>
            Saturday: 10:00 AM - 2:00 PM<br>
            Sunday: Closed
          </p>
        </div>
      </div>
    </div>

    <div class="contact-form-section">
      <h2 style="margin-top: 0;">Send Us a Message</h2>
      
      <form id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
        <div class="form-group">
          <label for="name">Full Name *</label>
          <input type="text" id="name" name="name" required>
        </div>

        <div class="form-group">
          <label for="email">Email Address *</label>
          <input type="email" id="email" name="email" required>
        </div>

        <div class="form-group">
          <label for="affiliation">Affiliation / Organization</label>
          <input type="text" id="affiliation" name="affiliation">
        </div>

        <div class="form-group">
          <label for="subject">Subject *</label>
          <select id="subject" name="subject" required>
            <option value="">Select a subject</option>
            <option value="collaboration">Research Collaboration</option>
            <option value="student">Student Opportunities</option>
            <option value="visit">Lab Visit</option>
            <option value="seminar">Seminar/Talk Invitation</option>
            <option value="media">Media Inquiry</option>
            <option value="other">Other</option>
          </select>
        </div>

        <div class="form-group">
          <label for="message">Message *</label>
          <textarea id="message" name="message" required></textarea>
        </div>

        <button type="submit" class="submit-btn">Send Message</button>
      </form>

      <p style="font-size: 0.9rem; color: #777; margin-top: 1rem; text-align: center;">
        * Required fields
      </p>
    </div>
  </div>

  <div class="social-section" style="text-align: center; margin: 4rem 0;">
    <h2>Connect With Us</h2>
    <div class="social-links">
      <a href="https://twitter.com/miraivisionlab" target="_blank" class="social-link" title="Twitter">
        <i class="fab fa-twitter"></i>
      </a>
      <a href="https://linkedin.com/company/miraivisionlab" target="_blank" class="social-link" title="LinkedIn">
        <i class="fab fa-linkedin"></i>
      </a>
      <a href="https://github.com/miraivisionlab" target="_blank" class="social-link" title="GitHub">
        <i class="fab fa-github"></i>
      </a>
      <a href="https://youtube.com/@miraivisionlab" target="_blank" class="social-link" title="YouTube">
        <i class="fab fa-youtube"></i>
      </a>
      <a href="mailto:info@miraivision.lab" class="social-link" title="Email">
        <i class="fas fa-envelope"></i>
      </a>
    </div>
  </div>

  <div class="map-container">
    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3022.1841!2d-73.9875!3d40.7484!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zM40zMCcxOC4yIk4gNzPCsDU5JzE1LjAiVw!5e0!3m2!1sen!2sus!4v1234567890"
      loading="lazy"
      referrerpolicy="no-referrer-when-downgrade"
      title="MIRAI VISION LAB Location">
    </iframe>
  </div>

  <div class="directions-section">
    <h3>🚗 Directions to Our Lab</h3>
    <ul class="directions-list">
      <li><strong>By Car:</strong> Take Highway 101 to Exit 25, follow signs to University Campus. Parking available in Structure P3.</li>
      <li><strong>By Public Transit:</strong> Take Metro Line 3 to University Station. Lab is a 5-minute walk from the station.</li>
      <li><strong>By Bus:</strong> Routes 42, 67, and 89 stop directly at the Engineering Building.</li>
      <li><strong>From Airport:</strong> Approximately 30 minutes by taxi or rideshare. Airport shuttle service also available.</li>
      <li><strong>Campus Map:</strong> Building XYZ is located in the north section of campus, near the Computer Science Department.</li>
    </ul>
  </div>

  <div class="visiting-info" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 3rem; border-radius: 12px; text-align: center; margin: 4rem 0;">
    <h2 style="color: white; margin: 0 0 1rem 0;">Planning to Visit?</h2>
    <p style="font-size: 1.1rem; margin: 0 0 2rem 0; max-width: 600px; margin-left: auto; margin-right: auto;">
      We welcome visitors! Please email us at least one week in advance to schedule a lab tour or meeting. 
      Visitors must check in at the main building reception upon arrival.
    </p>
    <a href="mailto:info@miraivision.lab?subject=Lab Visit Request" style="display: inline-block; padding: 0.75rem 2rem; background: white; color: #667eea; text-decoration: none; border-radius: 6px; font-weight: 600; transition: transform 0.3s ease;">
      Request a Visit
    </a>
  </div>

  <div class="opportunities-link" style="background: #f8f9fa; padding: 2rem; border-radius: 12px; text-align: center; margin: 4rem 0;">
    <h3>Interested in Joining Our Team?</h3>
    <p style="color: #555; margin: 1rem 0;">
      We're always looking for talented PhD students, postdocs, and research collaborators.
    </p>
    <a href="/team/" style="color: #667eea; font-weight: 600; text-decoration: none;">
      Learn more about opportunities →
    </a>
  </div>
</div>

<script>
document.getElementById('contactForm').addEventListener('submit', function(e) {
  // Form submission handling
  // If using Formspree, it will handle the submission automatically
  // You can add custom validation or success messages here
  
  console.log('Form submitted');
});
</script>

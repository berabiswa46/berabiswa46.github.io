---
layout: page
title: team
permalink: /team/
description: Meet the brilliant minds behind MIRAI VISION LAB
nav: true
nav_order: 2
---

<style>
.team-section {
  margin: 3rem 0;
}

.team-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.team-card {
  background: #fff;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.team-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.15);
}

.team-card-image {
  width: 100%;
  height: 300px;
  object-fit: cover;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.team-card-content {
  padding: 1.5rem;
}

.team-card-name {
  font-size: 1.3rem;
  font-weight: 600;
  margin: 0 0 0.5rem 0;
  color: #2c3e50;
}

.team-card-role {
  color: #0066cc;
  font-weight: 500;
  margin: 0 0 0.5rem 0;
}

.team-card-research {
  font-size: 0.9rem;
  color: #555;
  margin: 0.5rem 0;
  line-height: 1.5;
}

.team-card-contact {
  margin-top: 1rem;
  padding-top: 1rem;
  border-top: 1px solid #eee;
}

.team-card-contact a {
  color: #0066cc;
  text-decoration: none;
  font-size: 0.9rem;
  margin-right: 1rem;
}

.team-card-contact a:hover {
  text-decoration: underline;
}

.professor-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(400px, 1fr));
  gap: 3rem;
  margin: 2rem 0;
}

.professor-card {
  background: #fff;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.professor-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.15);
}

.professor-image {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  margin: 0 auto 1.5rem;
  display: block;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.professor-name {
  font-size: 1.5rem;
  font-weight: 600;
  text-align: center;
  margin: 0 0 0.5rem 0;
  color: #2c3e50;
}

.professor-title {
  text-align: center;
  color: #0066cc;
  font-weight: 500;
  margin: 0 0 1rem 0;
}

.professor-bio {
  line-height: 1.7;
  color: #555;
  margin: 1rem 0;
}

.professor-interests {
  margin: 1rem 0;
}

.professor-interests h4 {
  font-size: 1rem;
  font-weight: 600;
  margin: 0 0 0.5rem 0;
}

.professor-interests ul {
  margin: 0;
  padding-left: 1.5rem;
}

.professor-contact {
  margin-top: 1.5rem;
  padding-top: 1.5rem;
  border-top: 2px solid #eee;
  text-align: center;
}

.professor-contact a {
  display: inline-block;
  margin: 0.5rem;
  padding: 0.5rem 1rem;
  background: #0066cc;
  color: white;
  text-decoration: none;
  border-radius: 6px;
  font-size: 0.9rem;
  transition: background 0.3s ease;
}

.professor-contact a:hover {
  background: #0052a3;
}

@media (max-width: 768px) {
  .team-grid, .professor-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="team-intro" style="text-align: center; margin: 2rem 0 4rem 0;">
  <h1>Our Team</h1>
  <p style="font-size: 1.2rem; color: #555; max-width: 800px; margin: 1rem auto;">
    MIRAI VISION LAB brings together talented researchers, students, and collaborators 
    from diverse backgrounds, united by a passion for advancing computer vision and AI.
  </p>
</div>

---

## Principal Investigators

<div class="professor-grid">
  <div class="professor-card">
    <img src="{{ '/assets/img/team/professor1.jpg' | relative_url }}" alt="Professor 1" class="professor-image">
    <h3 class="professor-name">Dr. [Name Placeholder]</h3>
    <p class="professor-title">Professor & Lab Director</p>
    
    <div class="professor-bio">
      <p>Dr. [Name] is a distinguished researcher in computer vision and machine learning with over 15 years of experience. Their work focuses on deep learning architectures for visual understanding and has been published in top-tier venues including CVPR, ICCV, and NeurIPS.</p>
    </div>
    
    <div class="professor-interests">
      <h4>Research Interests:</h4>
      <ul>
        <li>Deep Learning for Computer Vision</li>
        <li>3D Scene Understanding</li>
        <li>Medical Image Analysis</li>
        <li>Neural Architecture Search</li>
      </ul>
    </div>
    
    <div class="professor-contact">
      <a href="mailto:professor1@university.edu">Email</a>
      <a href="https://scholar.google.com" target="_blank">Google Scholar</a>
      <a href="https://personal-website.com" target="_blank">Website</a>
    </div>
  </div>

  <div class="professor-card">
    <img src="{{ '/assets/img/team/professor2.jpg' | relative_url }}" alt="Professor 2" class="professor-image">
    <h3 class="professor-name">Dr. [Name Placeholder]</h3>
    <p class="professor-title">Associate Professor & Co-Director</p>
    
    <div class="professor-bio">
      <p>Dr. [Name] specializes in robotics and autonomous systems, with expertise in vision-based navigation and perception. They have led numerous projects in collaboration with industry partners and have received multiple best paper awards.</p>
    </div>
    
    <div class="professor-interests">
      <h4>Research Interests:</h4>
      <ul>
        <li>Robotic Vision & Perception</li>
        <li>Autonomous Systems</li>
        <li>SLAM and 3D Reconstruction</li>
        <li>Real-time Computer Vision</li>
      </ul>
    </div>
    
    <div class="professor-contact">
      <a href="mailto:professor2@university.edu">Email</a>
      <a href="https://scholar.google.com" target="_blank">Google Scholar</a>
      <a href="https://personal-website.com" target="_blank">Website</a>
    </div>
  </div>
</div>

---

## PhD Students

<div class="team-section">
  <div class="team-grid">
    <div class="team-card">
      <img src="{{ '/assets/img/team/phd1.jpg' | relative_url }}" alt="PhD Student 1" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">PhD Student (Year 3)</p>
        <p class="team-card-research">
          <strong>Research Area:</strong> Deep learning for medical image segmentation
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
          <a href="https://scholar.google.com" target="_blank">Scholar</a>
        </div>
      </div>
    </div>

    <div class="team-card">
      <img src="{{ '/assets/img/team/phd2.jpg' | relative_url }}" alt="PhD Student 2" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">PhD Student (Year 2)</p>
        <p class="team-card-research">
          <strong>Research Area:</strong> 3D vision and scene reconstruction
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
          <a href="https://scholar.google.com" target="_blank">Scholar</a>
        </div>
      </div>
    </div>

    <div class="team-card">
      <img src="{{ '/assets/img/team/phd3.jpg' | relative_url }}" alt="PhD Student 3" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">PhD Student (Year 1)</p>
        <p class="team-card-research">
          <strong>Research Area:</strong> Vision-language models and multimodal learning
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
          <a href="https://scholar.google.com" target="_blank">Scholar</a>
        </div>
      </div>
    </div>
  </div>
</div>

---

## M.Tech Students

<div class="team-section">
  <div class="team-grid">
    <div class="team-card">
      <img src="{{ '/assets/img/team/mtech1.jpg' | relative_url }}" alt="M.Tech Student 1" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">M.Tech Student</p>
        <p class="team-card-research">
          <strong>Research Area:</strong> Object detection in autonomous vehicles
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
        </div>
      </div>
    </div>

    <div class="team-card">
      <img src="{{ '/assets/img/team/mtech2.jpg' | relative_url }}" alt="M.Tech Student 2" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">M.Tech Student</p>
        <p class="team-card-research">
          <strong>Research Area:</strong> Facial recognition and biometric systems
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
        </div>
      </div>
    </div>
  </div>
</div>

---

## M.Sc Students

<div class="team-section">
  <div class="team-grid">
    <div class="team-card">
      <img src="{{ '/assets/img/team/msc1.jpg' | relative_url }}" alt="M.Sc Student 1" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">M.Sc Student</p>
        <p class="team-card-research">
          <strong>Research Area:</strong> Video analysis and action recognition
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
        </div>
      </div>
    </div>

    <div class="team-card">
      <img src="{{ '/assets/img/team/msc2.jpg' | relative_url }}" alt="M.Sc Student 2" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">M.Sc Student</p>
        <p class="team-card-research">
          <strong>Research Area:</strong> Image enhancement and restoration
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
        </div>
      </div>
    </div>
  </div>
</div>

---

## Project Students

<div class="team-section">
  <div class="team-grid">
    <div class="team-card">
      <img src="{{ '/assets/img/team/project1.jpg' | relative_url }}" alt="Project Student 1" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">Project Student</p>
        <p class="team-card-research">
          <strong>Project:</strong> Real-time object tracking system
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
        </div>
      </div>
    </div>

    <div class="team-card">
      <img src="{{ '/assets/img/team/project2.jpg' | relative_url }}" alt="Project Student 2" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">Project Student</p>
        <p class="team-card-research">
          <strong>Project:</strong> AI-powered image classification app
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
        </div>
      </div>
    </div>

    <div class="team-card">
      <img src="{{ '/assets/img/team/project3.jpg' | relative_url }}" alt="Project Student 3" class="team-card-image">
      <div class="team-card-content">
        <h3 class="team-card-name">[Student Name]</h3>
        <p class="team-card-role">Project Student</p>
        <p class="team-card-research">
          <strong>Project:</strong> Drone-based surveillance system
        </p>
        <div class="team-card-contact">
          <a href="mailto:student@university.edu">Email</a>
        </div>
      </div>
    </div>
  </div>
</div>

---

<div class="join-us" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 3rem; border-radius: 12px; text-align: center; margin: 4rem 0;">
  <h2 style="color: white; margin: 0 0 1rem 0;">Join Our Team!</h2>
  <p style="font-size: 1.1rem; margin: 0 0 2rem 0; max-width: 600px; margin-left: auto; margin-right: auto;">
    We are always looking for passionate and talented individuals to join MIRAI VISION LAB. 
    If you're interested in cutting-edge research in computer vision and AI, we'd love to hear from you!
  </p>
  <a href="/contact/" style="display: inline-block; padding: 0.75rem 2rem; background: white; color: #667eea; text-decoration: none; border-radius: 6px; font-weight: 600; transition: transform 0.3s ease;">
    Contact Us
  </a>
</div>

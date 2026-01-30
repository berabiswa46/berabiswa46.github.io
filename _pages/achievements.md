---
layout: page
title: achievements
permalink: /achievements/
description: Awards, honors, grants, and milestones of MIRAI VISION LAB
nav: true
nav_order: 5
---

<style>
.achievement-section {
  margin: 3rem 0;
}

.timeline {
  position: relative;
  padding: 2rem 0;
}

.timeline::before {
  content: '';
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 4px;
  height: 100%;
  background: linear-gradient(180deg, #667eea 0%, #764ba2 100%);
}

.timeline-item {
  display: flex;
  margin: 2rem 0;
  position: relative;
}

.timeline-item:nth-child(odd) {
  flex-direction: row;
}

.timeline-item:nth-child(even) {
  flex-direction: row-reverse;
}

.timeline-content {
  width: 45%;
  padding: 1.5rem;
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  position: relative;
}

.timeline-date {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  background: #667eea;
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-weight: 600;
  white-space: nowrap;
  z-index: 2;
}

.achievement-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.achievement-card {
  background: #fff;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border-left: 4px solid #667eea;
}

.achievement-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.15);
}

.achievement-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.achievement-title {
  font-size: 1.3rem;
  font-weight: 600;
  margin: 1rem 0 0.5rem 0;
  color: #2c3e50;
}

.achievement-description {
  color: #555;
  line-height: 1.6;
}

.achievement-meta {
  margin-top: 1rem;
  padding-top: 1rem;
  border-top: 1px solid #eee;
  font-size: 0.9rem;
  color: #777;
}

.stats-highlight {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 3rem;
  border-radius: 12px;
  text-align: center;
  margin: 3rem 0;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2rem;
  margin-top: 2rem;
}

.stat-box {
  padding: 1.5rem;
}

.stat-number {
  font-size: 3rem;
  font-weight: 700;
  margin: 0;
}

.stat-label {
  font-size: 1.1rem;
  margin: 0.5rem 0 0 0;
  opacity: 0.9;
}

@media (max-width: 768px) {
  .timeline::before {
    left: 20px;
  }
  
  .timeline-item {
    flex-direction: column !important;
    padding-left: 50px;
  }
  
  .timeline-content {
    width: 100%;
  }
  
  .timeline-date {
    left: 20px;
    transform: none;
  }
}
</style>

<div class="page-intro" style="text-align: center; margin: 2rem 0 4rem 0;">
  <h1>Achievements & Milestones</h1>
  <p style="font-size: 1.2rem; color: #555; max-width: 800px; margin: 1rem auto;">
    Celebrating our accomplishments in research excellence, innovation, and impact
  </p>
</div>

<div class="stats-highlight">
  <h2 style="margin: 0 0 2rem 0;">Our Impact at a Glance</h2>
  <div class="stats-grid">
    <div class="stat-box">
      <p class="stat-number">50+</p>
      <p class="stat-label">Published Papers</p>
    </div>
    <div class="stat-box">
      <p class="stat-number">$3.5M</p>
      <p class="stat-label">Research Funding</p>
    </div>
    <div class="stat-box">
      <p class="stat-number">15+</p>
      <p class="stat-label">Awards Received</p>
    </div>
    <div class="stat-box">
      <p class="stat-number">3</p>
      <p class="stat-label">Patent Applications</p>
    </div>
  </div>
</div>

---

## 🏆 Awards & Honors

<div class="achievement-section">
  <div class="achievement-grid">
    <div class="achievement-card">
      <div class="achievement-icon">🥇</div>
      <h3 class="achievement-title">Best Paper Award</h3>
      <p class="achievement-description">
        "Advanced Deep Learning for Medical Image Segmentation" received the Best Paper Award at International Conference on Computer Vision (ICCV) 2025
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> October 2025<br>
        <strong>Recipient:</strong> Dr. [Professor Name], [PhD Student]
      </div>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">⭐</div>
      <h3 class="achievement-title">Outstanding Research Award</h3>
      <p class="achievement-description">
        Lab recognized with University-wide Outstanding Research Team Award for contributions to autonomous vehicle perception
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> March 2025<br>
        <strong>Institution:</strong> University Research Office
      </div>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">🎓</div>
      <h3 class="achievement-title">PhD Excellence Award</h3>
      <p class="achievement-description">
        [PhD Student Name] received the prestigious Doctoral Excellence Award for dissertation on 3D scene reconstruction
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> December 2025<br>
        <strong>Institution:</strong> Graduate School
      </div>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">🌟</div>
      <h3 class="achievement-title">Young Researcher Award</h3>
      <p class="achievement-description">
        Recognition for innovative work in neural radiance fields and novel view synthesis
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> June 2025<br>
        <strong>Organization:</strong> International AI Society
      </div>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">🔬</div>
      <h3 class="achievement-title">Innovation Excellence Award</h3>
      <p class="achievement-description">
        Recognized for developing breakthrough real-time video analysis system with industry applications
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> September 2025<br>
        <strong>Organization:</strong> National Innovation Foundation
      </div>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">💡</div>
      <h3 class="achievement-title">Best Demo Award</h3>
      <p class="achievement-description">
        Interactive AR demonstration won Best Demo at Computer Vision and Pattern Recognition (CVPR) conference
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> June 2024<br>
        <strong>Conference:</strong> CVPR 2024
      </div>
    </div>
  </div>
</div>

---

## 💰 Research Grants

<div class="achievement-section">
  <div class="timeline">
    <div class="timeline-item">
      <span class="timeline-date">Jan 2026</span>
      <div class="timeline-content">
        <h3>NSF CAREER Award</h3>
        <p><strong>Amount:</strong> $600,000</p>
        <p><strong>Duration:</strong> 5 years</p>
        <p><strong>Project:</strong> Advanced 3D Vision and Reconstruction Technologies</p>
        <p>Supporting fundamental research in neural 3D representations and real-time rendering</p>
      </div>
    </div>

    <div class="timeline-item">
      <span class="timeline-date">Oct 2025</span>
      <div class="timeline-content">
        <h3>NIH Research Grant</h3>
        <p><strong>Amount:</strong> $800,000</p>
        <p><strong>Duration:</strong> 3 years</p>
        <p><strong>Project:</strong> AI-Powered Medical Imaging for Disease Detection</p>
        <p>Developing diagnostic tools for early cancer detection using deep learning</p>
      </div>
    </div>

    <div class="timeline-item">
      <span class="timeline-date">Mar 2025</span>
      <div class="timeline-content">
        <h3>DoT Autonomous Vehicle Grant</h3>
        <p><strong>Amount:</strong> $1,200,000</p>
        <p><strong>Duration:</strong> 3 years</p>
        <p><strong>Project:</strong> Vision Systems for Autonomous Transportation</p>
        <p>Funding robust perception algorithms for self-driving vehicles</p>
      </div>
    </div>

    <div class="timeline-item">
      <span class="timeline-date">Sep 2024</span>
      <div class="timeline-content">
        <h3>Industry Partnership - TechVision Corp</h3>
        <p><strong>Amount:</strong> $500,000</p>
        <p><strong>Duration:</strong> 2 years</p>
        <p><strong>Project:</strong> Real-time Object Detection for Industrial Automation</p>
        <p>Collaborative research on computer vision for manufacturing</p>
      </div>
    </div>

    <div class="timeline-item">
      <span class="timeline-date">June 2024</span>
      <div class="timeline-content">
        <h3>University Research Seed Grant</h3>
        <p><strong>Amount:</strong> $150,000</p>
        <p><strong>Duration:</strong> 1 year</p>
        <p><strong>Project:</strong> Multimodal Learning for Vision-Language Tasks</p>
        <p>Exploring integration of visual and textual information</p>
      </div>
    </div>
  </div>
</div>

---

## 📰 Media Coverage

<div class="achievement-section">
  <div class="achievement-grid">
    <div class="achievement-card" style="border-left-color: #e74c3c;">
      <h3 class="achievement-title">Tech News Daily</h3>
      <p class="achievement-description">
        "MIRAI VISION LAB's breakthrough in medical AI could revolutionize cancer diagnosis"
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> November 2025<br>
        <a href="#" target="_blank">Read Article →</a>
      </div>
    </div>

    <div class="achievement-card" style="border-left-color: #3498db;">
      <h3 class="achievement-title">Science Today Magazine</h3>
      <p class="achievement-description">
        Featured cover story on autonomous vehicle perception research
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> August 2025<br>
        <a href="#" target="_blank">Read Article →</a>
      </div>
    </div>

    <div class="achievement-card" style="border-left-color: #2ecc71;">
      <h3 class="achievement-title">University Press Release</h3>
      <p class="achievement-description">
        Lab's $3.5M in research funding highlights university's AI leadership
      </p>
      <div class="achievement-meta">
        <strong>Date:</strong> March 2025<br>
        <a href="#" target="_blank">Read Article →</a>
      </div>
    </div>
  </div>
</div>

---

## 📜 Patents & Intellectual Property

<div class="achievement-section">
  <div class="achievement-grid">
    <div class="achievement-card">
      <div class="achievement-icon">📄</div>
      <h3 class="achievement-title">Patent Application: Medical Image Analysis System</h3>
      <p class="achievement-description">
        <strong>Application No:</strong> US 2025/0123456<br>
        <strong>Status:</strong> Pending<br>
        <strong>Inventors:</strong> Dr. [Professor], [PhD Student]<br>
        AI-powered diagnostic system for automated disease detection from medical images
      </p>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">📄</div>
      <h3 class="achievement-title">Patent Application: 3D Reconstruction Method</h3>
      <p class="achievement-description">
        <strong>Application No:</strong> US 2025/0234567<br>
        <strong>Status:</strong> Pending<br>
        <strong>Inventors:</strong> Dr. [Professor], [PhD Student]<br>
        Novel neural network architecture for real-time 3D scene reconstruction
      </p>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">📄</div>
      <h3 class="achievement-title">Patent Application: Object Tracking Algorithm</h3>
      <p class="achievement-description">
        <strong>Application No:</strong> US 2024/0345678<br>
        <strong>Status:</strong> Under Review<br>
        <strong>Inventors:</strong> Dr. [Professor], Team<br>
        Advanced multi-object tracking system for autonomous vehicles
      </p>
    </div>
  </div>
</div>

---

## 🎯 Competition Wins

<div class="achievement-section">
  <div class="achievement-grid">
    <div class="achievement-card">
      <div class="achievement-icon">🏆</div>
      <h3 class="achievement-title">ImageNet Challenge 2025</h3>
      <p class="achievement-description">
        <strong>Rank:</strong> 2nd Place Overall<br>
        <strong>Category:</strong> Object Detection<br>
        Achieved state-of-the-art performance on large-scale visual recognition
      </p>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">🥈</div>
      <h3 class="achievement-title">MICCAI Medical Segmentation Challenge</h3>
      <p class="achievement-description">
        <strong>Rank:</strong> 1st Place<br>
        <strong>Year:</strong> 2025<br>
        Top performance in multi-organ segmentation from CT scans
      </p>
    </div>

    <div class="achievement-card">
      <div class="achievement-icon">🥉</div>
      <h3 class="achievement-title">Waymo Open Dataset Challenge</h3>
      <p class="achievement-description">
        <strong>Rank:</strong> 3rd Place<br>
        <strong>Category:</strong> 3D Object Detection<br>
        Recognized for innovative approach to autonomous driving perception
      </p>
    </div>
  </div>
</div>

---

<div class="cta-section" style="background: #f8f9fa; padding: 3rem; border-radius: 12px; text-align: center; margin: 4rem 0;">
  <h2>Be Part of Our Success Story</h2>
  <p style="font-size: 1.1rem; color: #555; margin: 1rem 0 2rem 0;">
    Join MIRAI VISION LAB and contribute to cutting-edge research that makes a difference
  </p>
  <a href="/contact/" class="btn btn-primary" style="padding: 0.75rem 2rem; background: #667eea; color: white; text-decoration: none; border-radius: 6px; font-weight: 600;">
    Get in Touch
  </a>
</div>

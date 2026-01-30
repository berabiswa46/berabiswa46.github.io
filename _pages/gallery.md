---
layout: page
title: gallery
permalink: /gallery/
description: Visual journey through MIRAI VISION LAB - events, research activities, and team moments
nav: true
nav_order: 6
---

<style>
.gallery-intro {
  text-align: center;
  margin: 2rem 0 3rem 0;
}

.filter-buttons {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 1rem;
  margin: 2rem 0;
}

.filter-btn {
  padding: 0.5rem 1.5rem;
  background: #fff;
  border: 2px solid #667eea;
  color: #667eea;
  border-radius: 25px;
  cursor: pointer;
  transition: all 0.3s ease;
  font-weight: 500;
}

.filter-btn:hover, .filter-btn.active {
  background: #667eea;
  color: white;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.gallery-item {
  position: relative;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  cursor: pointer;
  background: #f0f0f0;
}

.gallery-item:hover {
  transform: translateY(-8px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.2);
}

.gallery-item img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  display: block;
  transition: transform 0.3s ease;
}

.gallery-item:hover img {
  transform: scale(1.1);
}

.gallery-overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(to top, rgba(0,0,0,0.8) 0%, transparent 100%);
  color: white;
  padding: 1.5rem 1rem 1rem 1rem;
  transform: translateY(100%);
  transition: transform 0.3s ease;
}

.gallery-item:hover .gallery-overlay {
  transform: translateY(0);
}

.gallery-title {
  font-weight: 600;
  margin: 0 0 0.5rem 0;
  font-size: 1.1rem;
}

.gallery-date {
  font-size: 0.9rem;
  opacity: 0.9;
  margin: 0;
}

.category-badge {
  position: absolute;
  top: 1rem;
  right: 1rem;
  padding: 0.25rem 0.75rem;
  background: rgba(255,255,255,0.9);
  border-radius: 15px;
  font-size: 0.8rem;
  font-weight: 600;
  color: #667eea;
}

/* Lightbox styles */
.lightbox {
  display: none;
  position: fixed;
  z-index: 9999;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.95);
  align-items: center;
  justify-content: center;
}

.lightbox.active {
  display: flex;
}

.lightbox-content {
  max-width: 90%;
  max-height: 90%;
  position: relative;
}

.lightbox-content img {
  max-width: 100%;
  max-height: 90vh;
  object-fit: contain;
}

.lightbox-close {
  position: absolute;
  top: 2rem;
  right: 2rem;
  font-size: 3rem;
  color: white;
  cursor: pointer;
  z-index: 10000;
  background: rgba(0,0,0,0.5);
  width: 50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  line-height: 1;
}

.lightbox-caption {
  position: absolute;
  bottom: 2rem;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  background: rgba(0,0,0,0.7);
  padding: 1rem 2rem;
  border-radius: 8px;
  text-align: center;
}

@media (max-width: 768px) {
  .gallery-grid {
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 1rem;
  }
  
  .lightbox-close {
    top: 1rem;
    right: 1rem;
    font-size: 2rem;
    width: 40px;
    height: 40px;
  }
}
</style>

<div class="gallery-intro">
  <h1>Gallery</h1>
  <p style="font-size: 1.2rem; color: #555; max-width: 800px; margin: 1rem auto;">
    Capturing moments of innovation, collaboration, and discovery at MIRAI VISION LAB
  </p>
</div>

<div class="filter-buttons">
  <button class="filter-btn active" data-category="all">All</button>
  <button class="filter-btn" data-category="events">Events & Seminars</button>
  <button class="filter-btn" data-category="lab">Lab Activities</button>
  <button class="filter-btn" data-category="team">Team Outings</button>
  <button class="filter-btn" data-category="conferences">Conferences</button>
  <button class="filter-btn" data-category="equipment">Equipment & Facilities</button>
</div>

<div class="gallery-grid" id="galleryGrid">
  <!-- Events & Seminars -->
  <div class="gallery-item" data-category="events">
    <span class="category-badge">Events</span>
    <img src="{{ '/assets/img/gallery/event1.jpg' | relative_url }}" alt="Lab Opening Ceremony" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Lab Opening Ceremony</h3>
      <p class="gallery-date">January 15, 2026</p>
    </div>
  </div>

  <div class="gallery-item" data-category="events">
    <span class="category-badge">Events</span>
    <img src="{{ '/assets/img/gallery/event2.jpg' | relative_url }}" alt="Guest Lecture Series" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Guest Lecture on Deep Learning</h3>
      <p class="gallery-date">February 10, 2026</p>
    </div>
  </div>

  <div class="gallery-item" data-category="events">
    <span class="category-badge">Events</span>
    <img src="{{ '/assets/img/gallery/event3.jpg' | relative_url }}" alt="Workshop" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Computer Vision Workshop</h3>
      <p class="gallery-date">March 5, 2026</p>
    </div>
  </div>

  <!-- Lab Activities -->
  <div class="gallery-item" data-category="lab">
    <span class="category-badge">Lab</span>
    <img src="{{ '/assets/img/gallery/lab1.jpg' | relative_url }}" alt="Research Discussion" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Weekly Research Discussion</h3>
      <p class="gallery-date">Ongoing</p>
    </div>
  </div>

  <div class="gallery-item" data-category="lab">
    <span class="category-badge">Lab</span>
    <img src="{{ '/assets/img/gallery/lab2.jpg' | relative_url }}" alt="Coding Session" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Late Night Coding Session</h3>
      <p class="gallery-date">Various</p>
    </div>
  </div>

  <div class="gallery-item" data-category="lab">
    <span class="category-badge">Lab</span>
    <img src="{{ '/assets/img/gallery/lab3.jpg' | relative_url }}" alt="Experiment Setup" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Setting Up Experiments</h3>
      <p class="gallery-date">February 2026</p>
    </div>
  </div>

  <!-- Team Outings -->
  <div class="gallery-item" data-category="team">
    <span class="category-badge">Team</span>
    <img src="{{ '/assets/img/gallery/team1.jpg' | relative_url }}" alt="Team Dinner" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Team Celebration Dinner</h3>
      <p class="gallery-date">December 20, 2025</p>
    </div>
  </div>

  <div class="gallery-item" data-category="team">
    <span class="category-badge">Team</span>
    <img src="{{ '/assets/img/gallery/team2.jpg' | relative_url }}" alt="Hiking Trip" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Annual Hiking Trip</h3>
      <p class="gallery-date">November 2025</p>
    </div>
  </div>

  <div class="gallery-item" data-category="team">
    <span class="category-badge">Team</span>
    <img src="{{ '/assets/img/gallery/team3.jpg' | relative_url }}" alt="Game Night" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Friday Game Night</h3>
      <p class="gallery-date">Ongoing</p>
    </div>
  </div>

  <!-- Conferences -->
  <div class="gallery-item" data-category="conferences">
    <span class="category-badge">Conference</span>
    <img src="{{ '/assets/img/gallery/conf1.jpg' | relative_url }}" alt="CVPR 2025" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">CVPR 2025 Presentation</h3>
      <p class="gallery-date">June 2025</p>
    </div>
  </div>

  <div class="gallery-item" data-category="conferences">
    <span class="category-badge">Conference</span>
    <img src="{{ '/assets/img/gallery/conf2.jpg' | relative_url }}" alt="ICCV 2025" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">ICCV 2025 Best Paper Award</h3>
      <p class="gallery-date">October 2025</p>
    </div>
  </div>

  <div class="gallery-item" data-category="conferences">
    <span class="category-badge">Conference</span>
    <img src="{{ '/assets/img/gallery/conf3.jpg' | relative_url }}" alt="Poster Session" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Poster Presentation</h3>
      <p class="gallery-date">September 2025</p>
    </div>
  </div>

  <!-- Equipment & Facilities -->
  <div class="gallery-item" data-category="equipment">
    <span class="category-badge">Equipment</span>
    <img src="{{ '/assets/img/gallery/equip1.jpg' | relative_url }}" alt="GPU Cluster" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">GPU Computing Cluster</h3>
      <p class="gallery-date">Lab Facilities</p>
    </div>
  </div>

  <div class="gallery-item" data-category="equipment">
    <span class="category-badge">Equipment</span>
    <img src="{{ '/assets/img/gallery/equip2.jpg' | relative_url }}" alt="Robotics Setup" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Robotic Vision Platform</h3>
      <p class="gallery-date">Lab Facilities</p>
    </div>
  </div>

  <div class="gallery-item" data-category="equipment">
    <span class="category-badge">Equipment</span>
    <img src="{{ '/assets/img/gallery/equip3.jpg' | relative_url }}" alt="Camera Array" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">Multi-Camera Array Setup</h3>
      <p class="gallery-date">Lab Facilities</p>
    </div>
  </div>

  <div class="gallery-item" data-category="equipment">
    <span class="category-badge">Equipment</span>
    <img src="{{ '/assets/img/gallery/equip4.jpg' | relative_url }}" alt="Workstation" loading="lazy">
    <div class="gallery-overlay">
      <h3 class="gallery-title">High-Performance Workstations</h3>
      <p class="gallery-date">Lab Facilities</p>
    </div>
  </div>
</div>

<!-- Lightbox -->
<div class="lightbox" id="lightbox">
  <span class="lightbox-close" id="lightboxClose">&times;</span>
  <div class="lightbox-content">
    <img id="lightboxImg" src="" alt="">
    <div class="lightbox-caption" id="lightboxCaption"></div>
  </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  // Filter functionality
  const filterButtons = document.querySelectorAll('.filter-btn');
  const galleryItems = document.querySelectorAll('.gallery-item');
  
  filterButtons.forEach(button => {
    button.addEventListener('click', function() {
      const category = this.getAttribute('data-category');
      
      // Update active button
      filterButtons.forEach(btn => btn.classList.remove('active'));
      this.classList.add('active');
      
      // Filter items
      galleryItems.forEach(item => {
        if (category === 'all' || item.getAttribute('data-category') === category) {
          item.style.display = 'block';
          setTimeout(() => {
            item.style.opacity = '1';
            item.style.transform = 'scale(1)';
          }, 10);
        } else {
          item.style.opacity = '0';
          item.style.transform = 'scale(0.8)';
          setTimeout(() => {
            item.style.display = 'none';
          }, 300);
        }
      });
    });
  });
  
  // Lightbox functionality
  const lightbox = document.getElementById('lightbox');
  const lightboxImg = document.getElementById('lightboxImg');
  const lightboxCaption = document.getElementById('lightboxCaption');
  const lightboxClose = document.getElementById('lightboxClose');
  
  galleryItems.forEach(item => {
    item.addEventListener('click', function() {
      const img = this.querySelector('img');
      const title = this.querySelector('.gallery-title').textContent;
      const date = this.querySelector('.gallery-date').textContent;
      
      lightboxImg.src = img.src;
      lightboxCaption.innerHTML = `<strong>${title}</strong><br>${date}`;
      lightbox.classList.add('active');
      document.body.style.overflow = 'hidden';
    });
  });
  
  lightboxClose.addEventListener('click', closeLightbox);
  lightbox.addEventListener('click', function(e) {
    if (e.target === lightbox) {
      closeLightbox();
    }
  });
  
  function closeLightbox() {
    lightbox.classList.remove('active');
    document.body.style.overflow = 'auto';
  }
  
  // Keyboard navigation
  document.addEventListener('keydown', function(e) {
    if (e.key === 'Escape' && lightbox.classList.contains('active')) {
      closeLightbox();
    }
  });
});
</script>

<div class="gallery-note" style="background: #f8f9fa; padding: 2rem; border-radius: 12px; margin: 4rem 0; text-align: center;">
  <p style="margin: 0; color: #555;">
    📸 <strong>Note:</strong> This gallery showcases highlights from our lab activities. 
    For high-resolution images or media inquiries, please <a href="/contact/">contact us</a>.
  </p>
</div>

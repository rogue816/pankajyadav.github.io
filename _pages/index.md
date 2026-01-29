---
layout: home
title: Pankaj Yadav
permalink: /
---

<!-- Hero Section -->
<div style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
  <img src="images/healthcare.png" alt="Photo 1" style="flex: 1; max-width: 300px; height: auto; object-fit: cover;">
  <img src="images/pk.PNG" alt="Photo 2" style="flex: 1; max-width: 300px; height: auto; object-fit: cover;">
  
</div>



---
Hi! I am **Pankaj Yadav**, a PhD researcher. My work broadly spans ** Mitigating AI-based data biasdness**, which includes modeling algorithms through critical mathematical bottlenecks. I am passionate about developing and implementing interdisciplinary ideas that connect mathematics to computation and real-world problems.  

I recently worked on several AI projects, including **healthcare, solar energy, finance, sports science, and patient mobility data**. My focus is on improving **data efficiency, interpretability, and robustness** with statistical inference and its deep generative tools.

### Academic Background
- **PhD in Mathematics**, Indian Institute of Technology (IIT) Jodhpur, Mathematics Department  
- **M.Sc. in Mathematics**, IIT Jodhpur  
- **B.Sc. (Hons) in Mathematics**, University of Delhi  

### Philosophy & Approach
As uncertainty in the world increases—the inevitable Law of Thermodynamics—life will continue to surprise you. Keep Body, Soul, and Spirit in check, and the mortgage will be paid.

### Research Interests
- **Probabilistic Modeling & Statistical Inference**  
- **Deep Generative Models & AI-based Data Generation**  

### Recent Teaching
<ul>
  {% assign sorted_teaching = site.teaching | sort: 'date' | reverse %}
  {% for course in sorted_teaching limit: 3 %}
    <li>
      <a href="{{ course.url | relative_url }}"><strong>{{ course.title }}</strong></a> — {{ course.type }} ({{ course.date | date: "%Y" }})
    </li>
  {% endfor %}
</ul>

[View all teaching experience](/teaching/)


Contact: yadav.58@iitj.ac.in 



---

## Explore My Work
- [Publications](/publications)  
- [Talks](/talks)  
- [Teaching](/teaching)  
- [Portfolio](/portfolio)  
- [CV](/cv)

---

## Connect with Me
[Google Scholar](https://scholar.google.co.in/citations?hl=en&user=ejZNgHgAAAAJ) | 
[LinkedIn](https://www.linkedin.com/in/pankaj-yadav-867a40200/) | 
[GitHub](https://github.com/pankajyadav) | 
[ORCID](https://orcid.org/0009-0009-1437-5659?lang=en)

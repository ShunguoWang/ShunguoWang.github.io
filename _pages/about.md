---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.sw-carousel { position: relative; max-width: 100%; margin: 10px 0; }
.sw-carousel figure { margin: 0; }
.sw-slide { display: none; }
.sw-slide.is-active { display: block; }
.sw-slide img { width: 100%; display: block; border-radius: 4px; }
.sw-slide figcaption {
  text-align: center; font-size: 0.9rem; color: #555;
  padding: 6px 4px 0;
}
.sw-btn {
  position: absolute; top: 40%; transform: translateY(-50%);
  background: rgba(0,0,0,0.4); color: #fff; border: 0;
  font-size: 1.5rem; line-height: 1; padding: 6px 12px;
  cursor: pointer; border-radius: 4px; user-select: none;
}
.sw-btn:hover { background: rgba(0,0,0,0.65); }
.sw-prev { left: 8px; } .sw-next { right: 8px; }
.sw-dots { text-align: center; margin-top: 8px; }
.sw-dot {
  display: inline-block; width: 10px; height: 10px; margin: 0 4px;
  border-radius: 50%; background: #bbb; cursor: pointer;
}
.sw-dot.is-active { background: #555; }
</style>

<div class="sw-carousel" id="swCarousel">
  <figure class="sw-slide is-active">
    <img src="/images/SIO.jpeg" alt="SIO view from Scripps pier">
    <figcaption>SIO view from Scripps pier.</figcaption>
  </figure>
  <figure class="sw-slide">
    <img src="/images/Rock.jpeg" alt="Folded sedimentary rock at La Jolla beach">
    <figcaption>Folded sedimentary rock at La Jolla beach.</figcaption>
  </figure>
  <figure class="sw-slide">
    <img src="/images/Uppsala.jpeg" alt="Uppsala">
    <figcaption>Dark and beautiful Uppsala.</figcaption>
  </figure>
  <figure class="sw-slide">
    <img src="/images/RMT.jpeg" alt="RMT field work at Äspö, Sweden">
    <figcaption>RMT field work at Äspö, Sweden.</figcaption>
  </figure>
  <figure class="sw-slide">
    <img src="/images/Surf.jpeg" alt="Surf site in Lofoten, Norway">
    <figcaption>Surf site in Lofoten, Norway.</figcaption>
  </figure>
  <figure class="sw-slide">
    <img src="/images/LofotenRMT2.png" alt="CSRMT survey in Lofoten, Norway">
    <figcaption>CSRMT survey in Lofoten, Norway.</figcaption>
  </figure>
  <button class="sw-btn sw-prev" aria-label="Previous">&#10094;</button>
  <button class="sw-btn sw-next" aria-label="Next">&#10095;</button>
  <div class="sw-dots"></div>
</div>

<script>
(function () {
  var root = document.getElementById('swCarousel');
  if (!root) return;
  var slides = root.querySelectorAll('.sw-slide');
  var dotsWrap = root.querySelector('.sw-dots');
  var i = 0, timer;

  slides.forEach(function (_, idx) {
    var d = document.createElement('span');
    d.className = 'sw-dot' + (idx === 0 ? ' is-active' : '');
    d.addEventListener('click', function () { go(idx); reset(); });
    dotsWrap.appendChild(d);
  });
  var dots = dotsWrap.querySelectorAll('.sw-dot');

  function go(n) {
    slides[i].classList.remove('is-active');
    dots[i].classList.remove('is-active');
    i = (n + slides.length) % slides.length;
    slides[i].classList.add('is-active');
    dots[i].classList.add('is-active');
  }
  function reset() { clearInterval(timer); timer = setInterval(function () { go(i + 1); }, 5000); }

  root.querySelector('.sw-prev').addEventListener('click', function () { go(i - 1); reset(); });
  root.querySelector('.sw-next').addEventListener('click', function () { go(i + 1); reset(); });
  reset();
})();
</script>

<br style="line-height: 1;">
I am a geophysicist with a deep enthusiasm for developing innovative algorithms, acquiring geophysical datasets in exciting and challenging environments, and processing & inverting field data to unveil the fascinating narratives of Mother Earth. My expertise lies in electrical resistivity tomography, radio/audio-magnetotellurics, controlled source electromagnetics, and seismic refraction. Beyond my professional interests, I enjoy hiking, reading, yoga, skiing, climbing, practicing Tai Chi, and surfing (while I was in San Diego). 

<br> <b> <span style="font-size:150%"> Employment </span> </b> <br> 
<br> <b>2024 - </b> 
<br> Researcher, Geological Survey of Norway (NGU)
<br> Guest Researcher, Norwegian University of Science and Technology
<br class="line-space">
<br> <b>2020 - 2024</b> 
<br> Senior Researcher, Norwegian University of Science and Technology
<br> Collaborators: [Ståle E. Johansen](https://www.ntnu.no/ansatte/stale.johansen), [Martin Landrø](https://www.ntnu.no/ansatte/martin.landro)
<br class="line-space">
<br> <b>2018 - 2020</b> 
<br> Green Scholar (postdoc), Scripps Institution of Oceanography
<br> Advisor: [Steve Constable](https://marineemlab.ucsd.edu/steve/)
<br style="line-height: 1;">
<br> <b>2019</b> 
<br> Lecturer, Scripps Institution of Oceanography
<br style="line-height: 1;">
<br> <b>2018</b> 
<br> Visiting postdoc, Memorial University of Newfoundland
<br> Collaborators: [Colin G. Farquharson](https://www.esd.mun.ca/~farq/), [Hormoz Jahandari](https://www.mun.ca/math/people/ppl-postdoc/hormoz.php)
<br style="line-height: 1;">
<br> <b>2014, 2016</b> 
<br> EM geophysicist, Geological Survey of Sweden
<br> Collaborators: [Mehrdad Bastani](https://www.researchgate.net/profile/Mehrdad_Bastani), [Lena Persson](https://www.researchgate.net/profile/Lena_Persson2)

<br> <b> <span style="font-size:150%"> Education </span> </b> <br>
<br> <b>2013 - 2017</b> 
<br> Ph.D., Solid-Earth Physics, Uppsala University
<br> Advisors: [M. Bastani](https://www.researchgate.net/profile/Mehrdad_Bastani), [T. Kalscheuer](https://katalog.uu.se/profile/?id=N4-593), [A. Malehmir (lead)](https://katalog.uu.se/profile/?id=N3-1060), [L. B. Pedersen](https://www.researchgate.net/profile/Laust_Pedersen)
<br style="line-height: 1;">
<br> <b>2017</b> 
<br> Visiting graduate, Scripps Institution of Oceanography
<br> Host: [Steven Constable](https://marineemlab.ucsd.edu/steve/)
<br style="line-height: 1;">
<br> <b>2016</b> 
<br> Visiting graduate, Leicester University
<br> Host: [Max Moorkamp](https://www.geophysik.uni-muenchen.de/Members/moorkamp)
<br style="line-height: 1;">
<br> <b>2012 - 2013</b> 
<br> Ph.D. candidate, Applied Geophysics, Central South University
<br> Advisor: [Shikun Dai](https://www.researchgate.net/scientific-contributions/2107347787_Shikun_Dai)
<br style="line-height: 1;">
<br> <b>2009 - 2012</b> 
<br> M.S., Earth Exploration and Information Technology, Central South University
<br> Advisors: [Bin Xiong](https://www.researchgate.net/scientific-contributions/2078601980_Bin_Xiong), [Jishan He](http://en.csu.edu.cn/info/1010/1429.htm)
<br style="line-height: 1;">
<br> <b>2011</b> 
<br> Exchange program, Guilin University of Technology
<br style="line-height: 1;">
<br> <b>2005 - 2009</b> 
<br> B.S., Info-physics and Geomatics Engineering, Central South University
<br style="line-height: 1;">

[![Hits](https://hitscounter.dev/api/hit?url=https%3A%2F%2Fshunguowang.github.io&label=hits&icon=github&color=%2379C83D&message_color=%23555555)](https://hitscounter.dev)

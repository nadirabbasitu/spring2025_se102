---
layout: home
title: Home
nav_exclude: true
seo: 
  type: Course
  
---
<link rel="stylesheet" href="https://nadirabbasitu.github.io/spring2025_se102/assets/css/style.css">
<script>
  document.title = "{{ site.title }}"
</script>

<h1 class="mb-2" id="tagLine"></h1>


<!-- Announcements -->
{% if site.announcements %}
  <div class="fs-3" id="ann-btn">
    {{ site.announcements.last }}
    <a href="announcements/" class="btn btn-outline">Announcements</a>
  </div>
{% endif %}

<!-- Site Title -->
<h2 id="title"></h2>

<!-- Site Description -->
<p id="description"></p>

<!-- Guide Links -->
<a href="" id="guide"></a>

<div id="loader"></div>

<script src="https://nadirabbasitu.github.io/spring2025_se102/assets/js/library.js"></script>
<script>
        const siteButton = document.getElementById('menu-button');
        const siteNav = document.querySelector('.site-nav');

        let isVisible = false;

        siteButton.addEventListener('click', function(event) {
            event.preventDefault();
            if (isVisible) {
                siteNav.style.display = 'none';
                isVisible = false;
            } else {
                siteNav.style.display = 'block';
                isVisible = true;
            }
        });
    </script>
<script>
    library.staticData("{{site.courseDetails_sheet_url}}", "{{site.courseDetails}}","general_site_details", "indexView" ,{{site.site_mode_isOffline}}, "{{site.general_data_csv}}");
</script>

---
title: Tools
parent: Details
nav_order: 4
description: >-
    Tools
---
{% assign imagePrefix = '/spring2025_se102/' %}
# Tools
{:.no_toc}

---
<link rel="stylesheet" href="{{ imagePrefix }}assets/css/style.css">

<p align='center' style="background-color:black;">
  <img src='{{ imagePrefix }}assets/images/policy/tools.png' />
</p>



[//]: # (![image]&#40;/assets/images/policy/tools.png&#41;)

<a href="" class="btn btn-outline h6" id="guide_for_tools_url">Guide for Tools</a>
<a href="" class="btn btn-outline h6" id="reading_material_for_github_url">Reading Material for GitHub</a>

<div id="loader"></div>

<script src="../assets/js/library.js"></script>
<script>
    library.staticData("{{site.courseDetails_sheet_url}}", "{{site.courseDetails}}","general_site_details", "tools" ,{{site.site_mode_isOffline}}, "{{site.general_data_csv}}");
</script>

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
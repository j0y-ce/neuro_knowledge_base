---
layout: post
title: "MRI Sequences- DWI"
date: 2024-11-03 08:44:38 -0400
category: subcategory-content-1
author: joyce
short-description: 
---

-----

DWI (Diffusion Weighted Imaging) is a sequence that measures the relative ease with which water molecules can move (ie. water diffusion). 
Areas of higher restriction to water movement have lower signal intensity, whereas areas of lower restriction to diffusion have higher signal intensity. 
However, in practice, DWI most often refers to a diffusion weighted sequence layered on top of T2* signals. 
Areas of high intensity on T2* will be attenuated according to their level of diffusion restriction but hypointense areas on T2* will not become more hyperintense with DWI. 
In practical terms, this means that all fluid starts with a hyperintense appearance (because of T2*) but areas of fluid with low restriction to diffusion (such as CSF) are highly attenuated by the contribution of DWI. 

Signal intensity in DWI therefore looks like this in different tissues:
-	Fat: low signal intensity (due to low water content of fat)
-	Soft tissues: intermediate signal intensity
-	Free fluid: low signal intensity (no restriction of water diffusion)

For CNS structures in DWI, both white and grey matter have intermediate signal intensity, but white matter is slightly more hypointense. 
CSF is usually attenuated to black because of its low restriction to diffusion. Areas of acute infarct, tumor or pus (restricted diffusion) will in general appear hyperintense on DWI because:
<ol>
  <li>The accumulation of fluid accumulation gives these areas a T2* high signal intensity </li>
  <li>The fact that these areas are highly restrictive to water diffusion means that the originally high T2* is not attenuated by DWI</li>
</ol>

![Image]({{ site.baseurl }}/assets/DWI-density-scale.png){: width="800" }

In general, However, not all hyperintense structures in DWI correspond to an area of higher diffusion restriction. In some cases, structures appear hyperintense due to the contribution from T2*.  This phenomenon is called T2 shine-through.
In order to appreciate tissues represented by their actual diffusion coefficients without the influence of T2 signals, one can look at the ADC sequence (Apparent diffusion coefficient maps) that is even more sensitive to ischemic processes than DWI. 

![Image]({{ site.baseurl }}/assets/ADC-density-scale.png){: width="800" }


<a href="{{ site.baseurl }}/subcategory-content-1/MRI Sequences- T1">T1</a>

Read more <a href="https://radiopaedia.org/articles/mri-sequences-overview ">here</a> and <a href="https://radiopaedia.org/articles/diffusion-weighted-imaging-2 ">here </a>.

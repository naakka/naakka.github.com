---
layout: reveal
title: PHP Paas Comparison
meta:
  description: Comparing PHP Paas providers.
date: 2013-11-24
tags: [php, paas, google app engine, pagodabox, fortrabbit, jelastic, appfog]
---

{% include 'slides/title' %}

<section>
  <h2>Comparing different PHP PaaS* providers</h2>
  
  <ul>
    <li>Google App Engine</li>
    <li>PagodaBox</li>
    <li>Fort rabbit</li>
    <li>Jelastic</li>
    <li>AppFog</li>
  </ul>
  
  <p class="small">
    <small>* PaaS - Platform as a Service</small>
  </p>
</section>

<section>
  <h2>Things to consider</h2>
  
  <ul>
    <li>Servers physical location</li>
    <li>Ease of use</li>
    <li>Features</li>
    <li>Reliability</li>
    <li>Customer support</li>
  </ul>
</section>

<section>
  <h2>Google App Engine 1/2</h2>
  
  <ul>
    <li>Pros
      <ul>
        <li>Data stored in US or EU</li>
        <li>Scales easily and pretty much infinitely</li>
        <li>Very usable Task Queue</li>
        <li>Easy integration with Google services like user identification</li>
        <li>Good administration services like logging etc.</li>
        <li>Some good automatic Google enhancements, caches, DoS protection</li>
        <li>Memcache possible</li>
        <li>Automatic scaling within user defined limits</li>
				    <li>99.95% SLA (once out of preview)</li>
      </ul>
    </li>  
  </ul>
</section>

<section>
  <h2>Google App Engine 2/2</h2>
  
  <ul>
    <li>Cons
      <ul>
        <li>PHP support still in <em>preview</em></li>
        <li>No support for CURL, some API's need to be rewritten</li>
        <li>Files should be saved in database</li>
        <li>Only data storage option Google Cloud SQL</li>
      </ul>
    </li>
  </ul>
</section>

<section>
  <h2>Pagodabox</h2>
  
  <ul>
    <li>Pros
      <ul>
        <li>Great dashboard UI</li>
        <li>Integrates nicely with Github</li>
        <li>Memcache and Redis available</li>
      </ul>
    </li>
  
    <li>Cons
      <ul>
        <li>Data stored only in the US</li>
        <li>Somewhat unreliable</li>
      </ul>
    </li>
  </ul>
</section>

<section>
  <h2>Fortrabbit</h2>
  
  <ul>
    <li>Pros
      <ul>
        <li>Uses AWS</li>
        <li>Data stored in Ireland</li>
        <li>Berlin based Startup</li>
        <li>Many unhappy PagodaBox users have migrated to Fort Rabbit</li>
        <li>99.9% SLA</li>
      </ul>
    </li>
  
    <li>Cons
      <ul>
        <li>Only manual scaling</li>
        <li>MySQL ony database option</li>
      </ul>
    </li>
  </ul>
</section>

<section>
  <h2>Jelastic</h2>
  
  <ul>
    <li>Pros
      <ul>
        <li>Uses local web hosting providers, servers also in Helsinki hosted by Planeetta</li>
        <li>Easy, automatic scaling</li>
        <li>Both Apache and nginx available</li>
        <li>Many DB options: MySQL, MariaDB, PostgreSQL, MongoDB or CouchDB</li>
        <li>24/7 phone support available for 40€/month (price at Planeetta)</li>
        <li>High profile advisors: Monty Widenius, Rasmus Lehrdorf, Igor Sysoev...</li>
      </ul>
    </li>
  
    <li>Cons
      <ul>
        <li>Does it scale geographically?</li>
      </ul>
    </li>
  </ul>
</section>

<section>
  <h2>AppFog</h2>
  
  <ul>
    <li>Pros
      <ul>
        <li>Uses AWS infrastructure, EU available</li>
        <li>Lots of optional add-ons</li>
        <li>MySQL, MongoDB, Redis, Memcahced...</li>
      </ul>
    </li>
  
    <li>Cons
      <ul>
        <li>No file storage, save files in DB</li>
        
      </ul>
    </li>
  </ul>
  
</section>

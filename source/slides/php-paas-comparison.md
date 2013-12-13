---
layout: reveal
title: PHP Paas Comparison
meta:
  description: Comparing PHP Paas providers.
date: 2013-12-13
tags: [php, paas, google app engine, pagodabox, fortrabbit, jelastic, appfog]
---

{% include "slides/title.html" %}

<section>
  <h2>Comparing different PHP PaaS* providers</h2>
  
  <ul>
    <li>Google App Engine</li>
    <li>PagodaBox</li>
    <li>Fort rabbit</li>
    <li>Jelastic</li>
    <li>AWS Elastic Beanstalk</li>
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
    <li>Scalability</li>
    <li>Pricing</li>
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
        <li>Good email services, both sendin and receiving</li>
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
        <li>No support for cURL, some API's need to be rewritten</li>
        <li>Uploaded files cannot be saved as files</li>
        <li>Only data storage option Google Cloud SQL</li>
        <li>Extremely confusing pricing</li>
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
  <h2>AWS Elastic Beanstalk</h2>
  
  <ul>
    <li>Pros
      <ul>
        <li>Scalable Amazon infrastructure</li>
        <li>All Amazon EC2 features available, cdn, S3</li>
        <li>Static IP's available</li>
      </ul>
    </li>
  
    <li>Cons
      <ul>
        <li>Code needs some refactoring for saving files</li>
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
        <li>Manual scaling only</li>
      </ul>
    </li>
  </ul>
</section>

<section>
    <h2>Pricing</h2>
    
    <p class="small"><small>Comparing ~8GB 12GHz server on a monthly basis.</small></p>
  
    <table class="xsmall">
        <thead>
          <tr>
            <th></th><th>Web server</th><th>Database</th><th>Stored data</th><th>IP</th><th>Other costs</th><th></th>
          </tr>
        </thead>
        <tbody>
            <tr>
                <td>GAE</td>
                <td>$216 (8 * 1024MB, 2.4GHz)</td>
                <td>$88 (1GB ram, 2GB storage)</td>
                <td>$0.13/GB</td>
                <td>$39</td>
                <td>Sent emails, stored logs, DB writes/reads...</td>
                <td>~$350</td>
            </tr>
            <tr>
                <td>AWS EB</td>
                <td>$243 (7.5GB, 4 EC2 Compute Units)</td>
                <td>$104 1.7 GB memory, 1 ECU</td>
                <td>$0.11/GB</td>
                <td>$0</td>
                <td>Small amount for data transfer, possibly load balancing...</td>
                <td>~$350</td>
            </tr>
            <tr>
                <td>Jelastic (Planeetta)</td>
                <td>276,48€ (8GB, 12.8GHz)</td>
                <td></td>
                <td>0.07€/GB</td>
                <td>3.56€</td>
                <td></td>
                <td>~ 280€</td>
            </tr>
            <tr>
                <td>Fort Rabbit</td>
                <td>125€ (6 node high availability server)</td>
                <td>120€ (dedicated 1.7GB MySQL, 10GB storage)</td>
                <td>5GB for web, 10GB for db included</td>
                <td>??</td>
                <td>SSL 20€/month</td>
                <td>265€</td>
            </tr>
            <tr>
                <td>AppFog</td>
                <td>$380/month</td>
                <td>2GB included</td>
                <td></td>
                <td>??</td>
                <td>SSL 50€/month</td>
                <td>430€</td>
            </tr>
        </tbody>
    </table>

</section>

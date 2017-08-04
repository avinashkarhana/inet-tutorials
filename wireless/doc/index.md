---
layout: page
title: Wireless Tutorial for the INET Framework -- Part 1
tutorial: Wireless
---

In this tutorial, we show you how to build wireless simulations in the INET
Framework. The tutorial contains a series of simulation models numbered from 1 through 14.
The models are of increasing complexity -- they start from the basics and
in each step, they introduce new INET features and concepts related to wireless communication
networks.

This is an advanced tutorial, and it assumes that you are familiar with creating
and running simulations in OMNeT++ and  INET. If you aren't, you can check out
the <a href="https://omnetpp.org/doc/omnetpp/tictoc-tutorial/"
target="_blank">TicToc Tutorial</a> to get started with using OMNeT++. The <a
href="../../../doc/walkthrough/tutorial.html" target="_blank">INET Walkthrough</a>
is an introduction to INET and working with protocols.

If you need more information at any time, feel free to refer to the OMNeT++ and
INET documentation:

- <a href="https://omnetpp.org/doc/omnetpp/manual/usman.html" target="_blank">OMNeT++ User Manual</a>
- <a href="https://omnetpp.org/doc/omnetpp/api/index.html" target="_blank">OMNeT++ API Reference</a>
- <a href="https://omnetpp.org/doc/inet/api-current/inet-manual-draft.pdf" target="_blank">INET Manual draft</a>
- <a href="https://omnetpp.org/doc/inet/api-current/neddoc/index.html" target="_blank">INET Reference</a>

In the tutorial, each step is a separate configuration in the same omnetpp.ini file.
Steps build on each other, they extend the configuration of the previous step by adding
a few new lines. Consecutive steps mostly share the same network, defined in NED.

## Contents

<!-- find active submenu -->
{% for item in site.data.menu %}
  {% if item.submenu %}
    {% if page.tutorial == item.name %}{% assign activeSubmenu = item.submenu %}{% endif %}
  {% endif %}
{% endfor %}

<ul>
{% if activeSubmenu  %}
  {% for submenuitem in activeSubmenu %}
    {% unless submenuitem.separator %}
<li><a href="{{ submenuitem.link }}">{{ submenuitem.name }}</a></li>
    {% endunless %}
  {% endfor %}
{% endif %}
</ul>
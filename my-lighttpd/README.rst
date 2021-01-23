About
=====

A lite http server based on lighttpd.

Usage
-----

**Build**

::

  docker build -t my-httpd:v1.0 .


**Run**

::
  docker run -p 8001:8081 -it my-httpd:1.0


**Push**
::
  docker tag my-httpd:v1.0 quay.io/toongm/my-httpd:v1.0
  docker push quay.io/toongm/my-httpd:v1.0

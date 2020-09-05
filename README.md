# pdflibrary
Traning project for download web-pages to pdf files, using python, Jenkins, docker, k8s, etc

For using python script you must install:
python3 - pip3 pdf kit
apt - wkhtmltopdf

wkhtml PROBABLY must started with virtual display:
  1) apt install xvfb
  2) ln -s
  
  


apt-get install xvfb
printf '#!/bin/bash\nxvfb-run -a --server-args="-screen 0, 1024x768x24" /usr/bin/wkhtmltopdf -q $*' > /usr/bin/wkhtmltopdf.sh
sudo printf '#!/bin/bash\nxvfb-run -a --server-args="-screen 0, 1024x768x24" /usr/bin/wkhtmltopdf -q $*' > /usr/bin/wkhtmltopdf.sh
sudo chmod a+x /usr/bin/wkhtmltopdf.sh
ln -s /usr/bin/wkhtmltopdf.sh /usr/local/bin/wkhtmltopdf
sudo ln -s /usr/bin/wkhtmltopdf.sh /usr/local/bin/wkhtmltopdf
wkhtmltopdf http://www.google.com output.pdf
  



nxvfb-run -a --server-args="-screen 0, 1024x768x24"
xvfb-run -a --server-args="-screen 0, 1024x768x24" /usr/bin/wkhtmltopdf http://ya.ru ya.pdf

# CEMK_IT

mkdir pixel3
cd pixel3
wget -q https://digitalcorpora.s3.amazonaws.com/corpora/mobile/android_10/Non-Cellebrite%20Extraction/Pixel%203.zip
ls Pixel\ 3.zip -l


https://linuxhint.com/kali_linux_top_forensic_tools/#:~:text=The%20hashdeep%20tool%20is%20a,are%20generated%20with%20every%20output.
https://digitalcorpora.org/corpora/cell-phones/

hashdeep Pixel\ 3.zip 
5247820897,9cc37ebbbc4e918ee5427de1fe1deecc,ca6918ef8b20486b6a5ded15609ac51318f377829480f93be3ba15364a8aa00a,/home/kali/pixel3/Pixel 3.zip

unzip -q Pixel\ 3.zip

echo "START aaa END bbb END" | grep -oP "START(.*)END“
echo "START aaa END bbb END" | grep -oP "START(.*?)END"


curl --no-progress-meter https://play.google.com/store/apps/details?id=com.twitter.android | grep -Pio 'itemprop="name"><span>Twitter</span>’
curl --no-progress-meter https://play.google.com/store/apps/details?id=com.twitter.android | grep -Pio 'itemprop="name"><span>\K.*?(?=</span>)’
echo "START aaa END START bbb END" | grep -oP 'START(.*)END’
echo "START aaa END START bbb END" | grep -oP 'START(.*?)END'


ls 'Pixel 3/data/data' \                                                           
| while read package; do \
curl --no-progress-meter https://play.google.com/store/apps/details?id=$package \
| grep -Pio '<div jsname="sngebd">\K.*?(?=</div>)'  | grep  -io money\
&& echo $package; \


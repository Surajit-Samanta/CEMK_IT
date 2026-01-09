# CEMK_IT

select  id, title, datetime(last_visit_time/1000000+strftime('%s','1601-01-01'), 'unixepoch', 'localtime') from urls;

select id, "url_ref_ID: " || url, datetime(visit_time/1000000+strftime('%s','1601-01-01'), 'unixepoch', 'localtime'), "From_visit: " || from_visit, 'Tran:' || transition , "Duration: " || (visit_duration/1000) from visits order by visit_time;

select  "url_id: " || id, url, title from urls where id=1;
<img width="562" height="53" alt="image" src="https://github.com/user-attachments/assets/2848c32c-489b-4259-a3e9-3f1ab628875a" />

select  "url_id: " || id, url, title from urls where id=2 or id=3 or id=4;
printf "%x" -2147483648
echo "$((0x80000000 & 0xff))“
https://source.chromium.org/chromium/chromium/src/+/main:ui/base/page_transition_types.h?q=page_transition_types.h
<img width="1290" height="143" alt="image" src="https://github.com/user-attachments/assets/96555118-36a7-4ffe-8b5a-82778d1cbbe7" />
select  "url_id: " || id, url, title from urls where id=5 or id=6;<img width="639" height="53" alt="image" src="https://github.com/user-attachments/assets/4529fbdd-7962-442f-a89f-f7eea9d6a687" />

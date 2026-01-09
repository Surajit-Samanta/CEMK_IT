# CEMK_IT

select  id, title, datetime(last_visit_time/1000000+strftime('%s','1601-01-01'), 'unixepoch', 'localtime') from urls;

select id, "url_ref_ID: " || url, datetime(visit_time/1000000+strftime('%s','1601-01-01'), 'unixepoch', 'localtime'), "From_visit: " || from_visit, 'Tran:' || transition , "Duration: " || (visit_duration/1000) from visits order by visit_time;



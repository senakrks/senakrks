curl \
  --data-urlencode sig="$(\
   echo '{"body":{"key":{"eldest_kid":"0101c88e73bc090ea8e25dfb8d9fd28eb3a6d22943091da5117790f6dea6f53b99010a","fingerprint":"8459a75b6b2cd548d99984d731efc5a02a751d48","host":"keybase.io","key_id":"31efc5a02a751d48","kid":"0101c88e73bc090ea8e25dfb8d9fd28eb3a6d22943091da5117790f6dea6f53b99010a","uid":"9c058e0a3048cdec121d65c761c96d19","username":"dissenot"},"service":{"name":"github","username":"senakrks"},"type":"web_service_binding","version":1},"ctime":1715950782,"expire_in":157680000,"prev":"a24b6a06ac35996abfcd04b676e4012bc47294805475f48384daa52ca0d5321c","seqno":2,"tag":"signature"}' | \
   gpg -u '8459a75b6b2cd548d99984d731efc5a02a751d48' -a --sign)" \
  --data-urlencode type="web_service_binding.github" \
  --data-urlencode csrf_token="lgHZIDljMDU4ZTBhMzA0OGNkZWMxMjFkNjVjNzYxYzk2ZDE5zmZHVJrOAxcEAMDEIFMRh0A269IQgyOates2DezkLPvcKt/VtJQ3SsN8OToD" \
  --data-urlencode plain_out="1" \
  --data-urlencode session="kyjEEJwFjgowSM3sEh1lx2HJbRnEEHu71KLz8f+00Wk4N2Pq7TM=" \
  --data-urlencode signing_kid="0101c88e73bc090ea8e25dfb8d9fd28eb3a6d22943091da5117790f6dea6f53b99010a" \
  --data-urlencode remote_username="senakrks" \
  https://keybase.io/_/api/1.0/sig/post.json

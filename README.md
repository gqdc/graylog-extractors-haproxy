## Graylog 6 extractors for HAProxy

These extractors are able to parse the standard HAProxy HTTP logs. Example log message:

    92.211.35.123:58507 [10/Jul/2024:08:15:48.478] fe-https-in~ backend1/server2 2055/0/0/160/2215 200 8638 - - ---- 1/1/0/1/0 0/0 "GET / HTTP/1.1"

Will extract fields `haproxy_client_ip`, `haproxy_request_date`, `haproxy_frontend_name`, `haproxy_backend_name`, `haproxy_server_name`, `haproxy_times`, `haproxy_status_code`, `haproxy_bytes_read`, `haproxy_http_request`, `haproxy_http_method`, `haproxy_http_path`, `haproxy_http_version`, `haproxy_tr`, `haproxy_tw`, `haproxy_tc`, `haproxy_tr`, `haproxy_ta`.

**Originally created by Daniel Kerwin (Gini GmbH).**

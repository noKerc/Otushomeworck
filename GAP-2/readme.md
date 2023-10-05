Добавлены 2 папки с именами infra и app , в них созданы дашборды infra-1 и app-1 соответсвенно. Фотографии дашбордов прилагаю в папке GAP-2.
1)Для CPU-total используется node_cpu_seconds_total с Legend {{instance}} ,но наблюдается проблема с дублированием айпи адрессов по несколько раз.
2)Для Network используется node_network_receive_bytes_total с Legend {{instance}}.
3)Для RAM используется node_memory_MemTotal_bytes с Legend {{instance}} с Unit bytes(IEC).
4)Для Disk Space Used используется 100 - ((node_filesystem_avail_bytes * 100) / node_filesystem_size_bytes) с Legend {{instance}} с Unit Percent (0-100).

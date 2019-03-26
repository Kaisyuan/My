# My
# select r.ROUTE_NAME,count(*) as count from jcfx_road_emergency j INNER JOIN rwp_route r ON j.ROUTE_NAME = r.ROUTE_ID where j.PLAN >= 1 group by ROUTE_NAME having count > 0 ORDER BY count DESC;
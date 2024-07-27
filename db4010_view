CREATE OR REPLACE VIEW dept_sum_vu (name, minsal, maxsal, avgsal, avgcomm, maxcomm) 
AS SELECT d.dname, MIN(e.sal), MAX(e.sal), ROUND (AVG(e.sal)) , ROUND (AVG(NVL(e.comm,0))) , MAX(e.comm)
FROM emp e, dept d
WHERE e.deptno = d.deptno 
GROUP BY d.dname; 

SELECT * FROM dept_sum_vu;

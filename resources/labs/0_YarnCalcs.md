YARN NM Properties			
yarn.nodemanager.resource.cpu-vcores	2		
yarn.nodemanager.resource.memory-mb	10752		changed from 3852, because we had more memory available
YARM RM Properties			
yarn.scheduler.minimum-allocation-vcores	1		
yarn.scheduler.maximum-allocation-vcores	4		
yarn.scheduler.increment-allocation-vcores	1		
yarn.scheduler.minimum-allocation-mb	1024		
yarn.scheduler.maximum-allocation-mb	2048		changed from because of recomandation 4939
yarn.scheduler.increment-allocation-mb	1024		
Task Container Settings		MIN	
mapreduce.map.memory.mb	1024	10,5			adjusted to 1024 (no value configured in CM)
mapreduce.map.java.opts.max.heap	800	MIN	
mapreduce.map.cpu.vcores	1	2		changed to 2
mapreduce.reduce.memory.mb	1024		
mapreduce.reduce.java.opts.max.heap	800		
mapreduce.reduce.cpu.vcores	1		
MapReduce AM Settings			
yarn.app.mapreduce.am.resource.mb	1		
yarn.app.mapreduce.am.resource.command-opts	800		
yarn.app.mapreduce.am.resource.cpu-vcores	1		
Gateway Settings			
-D mapreduce.map.memory.mb	2048			changed (no value configured in CM)
-D mapreduce.reduce.memory.mb	4096			changed (no value configured in CM)
-D mapreduce.map.java.opts.max.heap	1638,4		changed (no value configured in CM)
-D mapreduce.reduce.java.opts.max.heap	3276,8		changed (no value configured in CM)
-D mapreduce.job.maps	2		
mapreduce.job.reduces	2		

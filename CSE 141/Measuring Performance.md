## Latency (execution time)
- Time it takes to finish a fixed task
- Speed (time to drive from A to B on highway)
- Matters for applications like scientific programs

## Throughput (bandwidth)
- Number of tasks per unit time
- Bandwidth (number of lanes in highway)
- Matters for applications like web servers

### Example
How to measure the performance of moving people for 10 miles round trip?
- Car: capacity 5, speed 60 mph
	- speed = distance / time
	- time = distance / speed = 10 miles / 60 mph = $\frac{1}{6}$ hrs = 10 min
	- **latency = 20 min**
	- **Throughput = 3 trips * 5 people = 15 ppl / hr**
- Bus: capacity 60, speed 20 mph
	- time = distance / speed  = 10 / 20 = 1/2 hr
	- **latency = 60 min**
	- **throughput = 60 ppl / hr**
Fastest way to send 10TB of data from US to UK?
- FTP, SMB, Rsync, or other?
	- We prioritize **throughput** because we care about how long it takes for all 10TB to transfer
	- Speed: Even 1 Gbps transfer takes days
	- Thus overnight shipping is the fastest method

## Comparing Performance
### Speed Up




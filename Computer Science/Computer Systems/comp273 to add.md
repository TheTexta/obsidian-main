#comp273 

|Mapping Type|Index Bits?|Block Placement|Conflict Rate|Search Speed|
|---|---|---|---|---|
|**Direct-Mapped**|✅ Yes|One fixed line per block|❌ High|✅ Fast|
|**Set-Associative**|✅ Yes|One set → multiple lines|⚖️ Balanced|⚠️ Medium|
|**Fully Associative**|❌ No|Any line in cache|✅ Very low|❌ Slowest|
Average access time = Hit time + (miss penalty * miss rate)
![[Screenshot 2025-04-16 at 3.00.40 PM.png]]

translation lookaside buffer TLB caches recently used translations from virtual to physical

block size trend: As block size increases, **transfer efficiency improves**, but **latency, fragmentation, and waste can also increase**.

cache write policy: Write-thru versus write-back


cpue pipelining

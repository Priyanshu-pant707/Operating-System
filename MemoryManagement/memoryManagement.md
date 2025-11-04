# Memory Management

- it is module of os


## function :
 - memory allocation
 - memory deallocation
 - memory protection - segmentation fault.

## memory management techniquies :

1. Contiguous 
 - entire process should be stored on consecutive memory location
 - types :
      1. fixed partion->one partion one process -> fixed number of partition
         - internal fragmentation
      2. Variable partion -> new partition created -> size  of process.
         -  external fragmentation.
         - solution of external fragmentation is compaction.



```
Partition allocation policies :
1. first fit.
2. best fit.
3.  worst fit.

```
2. Non contiguous 
 
- entire process divided into partitions and each partition can be stored on any memory location.
- types : 
   1. Paging  :
      - process is divided in equal size of partitions called as pages
      - physical memory is divided in same equal size partitions call as of frames
      - pages are scattered in frames.
      - logical address ->  physical address  using mmu (memory management unit).
      - processor will have a view of process and its pages.
      - page table is used to map a process page to physical frame
      - number of entries in pahe table = number of pages in process.
      - os maintains a page table for each process.
      - Page table size= number of pages * 1 page table entry size.
      - page table entry size = (frame number + extra bits).
      
 

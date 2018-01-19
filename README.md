# pensieve

## Introduction
Pensieve is a centralized service providing distributed synchronization, inspired by chubby and zookeeper.

Pensieve shares the basic idea of chubby as prividing coarse-grained locking as well as reliable storage for a loosely-coupled distributed system.

It's different with Zookeeper in at least three aspects as bellow:
- Provide Linearizability semantic rather than Linearizable writes plus FIFO client order;
- Provide Coarse-grained locking API directly;
- Clients cache data in a consistent,  write-through cache held in memory.

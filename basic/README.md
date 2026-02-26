# 01

## Grid, Block, Thread (and Warp)
- **Grid** = multiple **blocks**, 
- **Block** = Group of **threads** - allowing **threads** within same block to communicate and share data quickly, has shared memory (visible to all threads in thread block)
- **Warp** = 32 (usually 32, but can be lower) **threads** in a block - CPU send execution to **warp**, not **thread** => 32 threads execute their instructions simultaneously (called active warp if a warp is allocated)
- **Thread** = individual worker executing a single calculation, has local memory and private to thread

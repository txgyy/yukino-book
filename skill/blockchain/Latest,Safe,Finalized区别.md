## Latest,Safe,Finalized区别

Safe and finalized commitment levels are determined by the completion of epochs. 
Let’s imagine the first three epochs (epoch 0, 1, and 2) after The Merge to visualize how safe and finalized blocks work.

Epoch 0 = blocks 0-31 \
Epoch 1 = blocks 32-63 \
Epoch 2 = blocks 64-95 \
Epoch 3 = blocks 96-127

Let’s assume the latest block is block 96, which marks the beginning of epoch 3 and the end of epoch 2.

Because block 96 includes attestations (i.e. votes from validators that signal the proposed canonical block head is true) for block 64, once the Beacon Chain receives attestations from two-thirds of the validators, block 64 is labeled as justified (safe).

Once block 64 is labeled is justified and marked safe, the previously justified block is marked as finalized. Because safe and finalized blocks occur at the beginning of epochs, block 32 (the first block of epoch 1) is marked finalized.

Here’s another way to visualize it if the current block number is 96:

Block 96 (start of epoch 3) = latest
Block 64 (start of epoch 2) = justified (safe)
Block 32 (start of epoch 1) = finalized

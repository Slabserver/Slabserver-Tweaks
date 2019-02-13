# Fish lag fix

In 1.13, fish could spawn in very large pack sizes, making it possible for 
several hundreds of them to spawn in a single cycle, many times above the mob cap.

This function removes naturally spawning fish when the number of natural fish exceeds 100.
Fish from a bucket or with a nametag are not removed.

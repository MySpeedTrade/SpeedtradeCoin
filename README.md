# SpeedtradeCoin Core [MSTC]
==========================
## What is SpeedtradeCoin? 
SpeedtradeCoin is a cryptocurrency like litecoin, although it does not use SHA256 as its proof of work (POW). Taking development cues from Tenebrix and Litecoin, SpeedtradeCoin currently employs a simplified variant of scrypt.

https://myspeedtrade.com/

 - Coin Name: SpeedtradeCoin
 - Currency unit : MSTC
 - Algorithm : Scrypt
 - Block Interval : 1 minute (60 seconds)
 - Difficulty Retarget : Every block (using Kimoto's Gravity Well)
 - Total supply : 25,000,000 MSTC
 - Max total Supply : 50,000,000 MSTC 
 - Premine: First block is 25,000,000 MSTC 
 - Bonus reward for block 2 to 50,000 of 2MSTC
 - Bonus reward for block 50,000 - 100,000 of 1.5MSTC
 - Bonus reward for block 100,000 - 600,000 of 1MSTC
 - Bonus reward for block 1,200,000 - 1,600,000 of 0.5 MSTC
 - Subsidy is cut in half every 200,000 blocks starting at block 1600000
  
### Overview plz make speedtradecoind/speedtradecoin-cli/speedtradecoin-qt

  The following are developer notes on how to build SpeedtradeCoin on your native platform. They are not complete guides, but include notes on the necessary libraries, compile flags, etc.

  - [OSX Build Notes](doc/build-osx.md)
  - [Unix Build Notes](doc/build-unix.md)
  - [Windows Build Notes](doc/build-msw.md)

 
# speedtradecoin.conf

  - listen=1
  - rpcallowip=127.0.0.1
  - rpcport=42244
  - port=42246
  - rpcuser=MSTCuser
  - rpcpassword=MSTCpassword


**DEBUG_LOCKORDER**

SpeedtradeCoin Core is a multithreaded application, and deadlocks or other multithreading bugs
can be very difficult to track down. Compiling with -DDEBUG_LOCKORDER (configure
CXXFLAGS="-DDEBUG_LOCKORDER -g") inserts run-time checks to keep track of what locks
are held, and adds warning to the debug.log file if inconsistencies are detected.

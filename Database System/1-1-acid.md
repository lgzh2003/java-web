##ACID
       
###Definition  
In computer science, **ACID** (**Atomicity**, **Consistency**, **Isolation**, **Durability**) is a set of properties of database transactions. In the context of databases, **a single logical operation on the data is called a transaction**.                           
ACID，指数据库事务正确执行的四个基本要素的缩写。包含：原子性（Atomicity）、一致性（Consistency）、隔离性（Isolation）、持久性（Durability）。一个支持事务（Transaction）的数据库，必需要        
具有这四种特性，否则在事务过程（Transaction processing）当中无法保证数据的正确性，交易过程极可能达不到交易方的要求。               
                    
####Atomicity                 
In a transaction involving two or more discrete pieces of information, **either all of the pieces are committed or none are**.               
整个事务中的所有操作，**要么全部完成，要么全部不完成**，不可能停滞在中间某个环节。事务在执行过程中发生错误，会被回滚（Rollback）到事务开始前的状态，就像这个事务从来没有执行过一样。              
             
####Consistency            
A transaction either creates a new and valid state of data, or, if any failure occurs, returns all data to its state before the transaction was started.               
事务的一致性是指事务的执行不能破坏数据库的一致性，一致性也称为完整性。**一个事务在执行后，数据库必须从一个一致性状态转变为另一个一致性状态**。                      
其主要特征是保护性和不变性(Preserving an Invariant)，以转账案例为例，假设有五个账户，每个账户余额是100元，那么五个账户总额是500元，如果在这个5个账户之间同时发生多个转账，无论并发多少个，       
比如在A与B账户之间转账5元，在C与D账户之间转账10元，在B与E之间转账15元，五个账户总额也应该还是500元，这就是保护性和不变性.            
      
####Isolation
A transaction in process and **not yet committed must remain isolated** from any other transaction.                 
事务的隔离型是指**并发的事务相互隔离，不能互相干扰**。             
         
####Durability           
**Committed data** is saved by the system such that, even in the event of a failure and system restart, the data is available in its correct state.          
事务的持久性是指**事务一旦提交，对数据的状态变更应该被永久保存**。              
           
              
                
                      
           
           



               
         

                 
          
         


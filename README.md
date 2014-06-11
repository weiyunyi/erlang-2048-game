**0 . prework**

    intall erlang and set erlang PATH.

**1. config**

- change your center name in game2048.hrl, format as : game2048_center@IP
- for example: game2048_center@127.0.0.1

    1.1 windows: 
	
	change ./bat/center_server.bat node name       : game2048_center@IP
	
    1.2 linux:
	
	change ./sh/start_server node's name       : game2048_center@IP


**2. compile**

2.1 windows:
		
		double click ./bat/compile.bat
  
   2.2 linux:
     	
		make 
     
**3.  set center_server up**
	
   3.1 windows:
     	
	double click ./bat/center_server.bat
  
   3.2 linux:
	
	./sh/start_server.sh
**4. run game2048 client**

4.1 windows:
     
	double click ./bat/player1.bat

4.2 linux:
	
	./sh/start_client.sh

**5. Tip**
	
-   5.1 press down 
   
    	|  Left:A | Right:D | Up:W  | Down:S  |

- 	5.2 Save game : File -> Save game
- 	5.3 play game with other : online -> signup (set a new name) -> click "<-" button right to begin

- 	5.4 chat with other : write msg in blew dialogue, print Enter to send msg.

-------------------------------------------------------------------------
If you just want to play alone, you can :
	
	erl -name test -pa "./ebin/"
    >application:start(game2048).
    >appliccation:stop(game2048).

---------------------------------------------------------------------------
Find work flow in  **[Wiki](https://github.com/zhongwencool/2048/wiki)**

 Html Doc generate by Erlang Edoc :**[Document](https://github.com/zhongwencool/2048/tree/master/doc)**
![gamepic](http://zhongwencool.qiniudn.com/erlang2048.png)
classDiagram
    Command <|.. AbstractCommand : implements
    List <|.. AbstractList : implements
    AbstractCommand <|-- BoardCommand
    AbstractCommand <|-- ProjectCommand
    AbstractCommand <|-- UserCommand
    Command <|-- HelpCommand
    AbstractList <|-- ArrayList
    AbstractList <|-- LinkedList
    Iterator <|.. ListIterator : implements
    class Command{
		    <<interface>>
				+execute()*
    }
    class AbstractCommand{
    		<<abstract>>
        #String menuTitle
        +AbstractCommand()
        #getMenus()*
        #processMenu()*
        +execute()
        -printMenus()
        -getMenuTitle()
        -isValidateMenu()
    }
    class List{
		    <<interface>>
				+execute()*
    }    
    class AbstractList{
    		<<abstract>>
        #String menuTitle
        +AbstractCommand()
        #getMenus()*
        #processMenu()*
        +execute()
        -printMenus()
        -getMenuTitle()
        -isValidateMenu()
    }
    class Iterator{
		    <<interface>>
				+execute()*
    }       
namespace Commands {
    class BoardCommand{
        -boardList : List
        -menus : String[]
        +BoardCommand()
        #getMenus()
        #processMenu()
        -addBoard()
        -listBoard()
        -viewBoard()
        -updateBoard()
        -deleteBoard()
    }
    class ProjectCommand{
        -projectList : List
        -userList : List 
        -menus : String[]
        #getMenus()
        #processMenu()
        -addProject()
        -listProject()
        -viewProject()
        -updateProject()
        -deleteProject()
        -addMembers()
        -deleteMemebers()
    }
    class UserCommand{
        -userList : List
        -menus : String[]
        #getMenus()
        #processMenu()
        -addUser()
        -listUser()
        -viewUser()
        -updateUser()
        -deleteUser()
    }
    class HelpCommand{
        +execute()
    }
}
namespace Util {
    class LinkedList{
    }
    class ArrayList{
    }
    class ListIterator{
    }
}




> I'm currently working on [@My Project](https://github.com/backnback/bitcamp-mystudy/tree/main/myapp).
> 
> 
> *PS: I haven't been very active on [lowlighter/metrics](https://github.com/lowlighter/metrics) recently, but I'm planning to work back on it once I finish [mizu.js](https://mizu.sh), which with [matcha.css](https://matcha.mizu.sh) and [@libs](https://github.com/lowlighter/libs) combined will make it easier to manage !*
> 
> *Thanks for your attention !*

[<img align="left" width="390" alt="🦑" src="https://gist.githubusercontent.com/lowlighter/3c6eaedf50273adfb7a510822672f570/raw/general.svg">](#)
[<img align="right" width="390" alt="🦑" src="https://gist.githubusercontent.com/lowlighter/3c6eaedf50273adfb7a510822672f570/raw/medias.svg?p">](#)
[<img align="right" width="390" height="80" alt="🦑" src="https://gist.githubusercontent.com/lowlighter/3c6eaedf50273adfb7a510822672f570/raw/placeholder.svg">](#)

[<img align="left" width="390" alt="🦑" src="https://gist.githubusercontent.com/lowlighter/3c6eaedf50273adfb7a510822672f570/raw/sponsors.svg">](https://github.com/sponsors/lowlighter)
[<img align="right" width="390" alt="🦑" src="https://gist.githubusercontent.com/lowlighter/3c6eaedf50273adfb7a510822672f570/raw/achievements.svg">](#)

[<img width="100%" height="1" alt="🦑" src="https://gist.githubusercontent.com/lowlighter/3c6eaedf50273adfb7a510822672f570/raw/placeholder.svg">](#)

[<img align="right" alt="🦑" src="https://github.com/lowlighter/lowlighter/assets/22963968/f03a6539-5f5e-4e29-8cc5-8f2138660440">](#)



<sub>These infographics were generated using [lowlighter/metrics](https://github.com/lowlighter/metrics)</sub>

<!-- Grizzco: https://user-images.githubusercontent.com/22963968/190084456-0e077445-abae-4355-8061-5f0830a48d6e.png -->
<!-- Until that day: https://user-images.githubusercontent.com/22963968/159836902-a7553777-f1e2-49ed-90fc-9721322b3f44.png -->
<!-- The betrayer: https://user-images.githubusercontent.com/22963968/155458995-e4c24fff-d667-48cd-a1ce-1f66cd233a14.png -->
<!-- The world ender: https://user-images.githubusercontent.com/22963968/130322172-4e4996cd-eb3d-4013-9fc2-47e573413310.png -->
<!-- Farewell Miura: https://user-images.githubusercontent.com/22963968/119890439-1ff29f00-bf38-11eb-8515-d0a9c3c8a6b6.png -->
<!-- First steps with JavaScript: https://user-images.githubusercontent.com/22963968/114021347-e3c48b80-9870-11eb-8bc8-998bf39b4d0d.png -->

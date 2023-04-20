这里是SUSTech java2课程 第二次作业 基于javafx和socket实现的井字棋游戏 

本项目实现了可以选择对手的联机对战

如有疑问可在issue中提出

以下为demo文件的readme文件内容

# Assignment 2 Tic-tac-toe Game

This is a template for CS209A-22fall, assignment 2.

## How to start?

### Install

Enter the [github repository ](https://github.com/Sustech-yx/Tic-tac-toe)and [fork](https://github.com/Sustech-yx/Tic-tac-toe/fork) the repo. Clone the repo to your local machine.

### Configure

After fork and clone the repository into your local machine, if you run it immediately, you will meet `IllegalStateException`. It is because `javaFX` cannot find the correct position of the resource file. With IntelliJ IDEA, you can Right click the resources dict and mark it as *resources*. 

![image-20221029213444154](README.assets/image-20221029213444154.png)

If the result seems like this, it means that you do the right thing.

![image-20221029213844851](README.assets/image-20221029213844851.png)

If you are using eclipse, you need to right-click Project>new>source folder, manually fill in the path of the resources directory, and then confirm.

### Start the game

The main function entry: `src/application/Main.java`.

![image-20220930180502858](README.assets/image-20220930180502858.png)

Now you can click the chessboard and play the game!

![image-20220930180659882](README.assets/image-20220930180659882.png)

## Java Version

The java version for reference. If you want to use another java language level, maybe there will be something wrong. Feel free to explore!

![image-20220930145108089](README.assets/image-20220930145108089.png)

You can use `System.out.println(com.sun.javafx.runtime.VersionInfo.getRuntimeVersion());` to check the version of `javafx`. The following screen-shot is the version of my machine.

![image-20221026155813168](README.assets/image-20221026155813168.png)

## Demo View

This is a demo view for the assignment. However, the basic functions are not complete yet. You should do it by yourself!

![image-20220930144914104](README.assets/image-20220930144914104.png)

## TODO

- [ ] Server (35pt.)
- [ ] Client/Player (35pt.)
- [x] GUI (15pt.)
- [ ] Exception Handling (15pt.)
- [ ] Bonus (15pt.)

## Hint

You need to first decouple the view and controller, divide the controller into two components: **client** and **server**, and then use **socket** to communicate between the two components to complete the basic functions.

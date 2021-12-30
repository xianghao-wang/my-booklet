# Java环境配置

平时使用的jdk及jdk管理☕️

## JDK主要特征

* **JDK8**

  * lambda表达式

    ```java
    List<Integer> l = new ArrayList<>();
    // add some elements
    // ...
    
    // sort via lamda expression
    l.sort((a, b) -> a - b);
    ```

    

  * 方法引用

* **JDK9**

  * jshell

* **JDK10**

  * ‼️**try-with-resources**

    ```java
    try (FileInputStream in = new FileInputStream("test.txt")) {
      // statements
    } catch (IOException e) {
      e.printStackTrace();
    }
    ```

    

* **JDK12,13,14**

  * 围绕着**enhanced switch**更新

    ```java
    Strring msg = switch (color) {
        case 0 -> "red";
        case 1 -> "green";
        case 2 -> "blue";
    };
    ```

    

## JDK发行商

* **Azul**: [link](https://www.azul.com/downloads/)
* **OpenJDK**: [link](https://www.openlogic.com/openjdk-downloads)

## JDK版本管理

* **jenv**(正在使用)
  * 需要自行下载jdk，然后手动将jdk路径添加到jenv
  * 命令很少，操作简洁
* **sdkman**
  * 集jdk下载，安装，切换，卸载为一体
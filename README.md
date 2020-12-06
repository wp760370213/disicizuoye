
# 实验内容
- 1.在桌面创建一个文本B，写入《长恨歌》。在创建一个空白的文本A
- 2.要求：
- 每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
- 允许提供输入参数，统计古诗中某个字或词出现的次数
- 考虑操作中可能出现的异常，在程序中设计异常处理程序
- 3.将处理后的信息存储到文件A中
# 实验目的
- 1.掌握字符串String及其方法的使用
- 2.掌握文件的读取/写入方法
- 3.掌握异常处理结构
#实验过程
1.编写student类 (1)属性：name(姓名)，major(专业)，stuNum(学号)，age(年龄) (2)通过Scanner类实例化学生信息，将学生信息输入进去 2.编写test(测试)类 (1)通过Fileinputstream读取文本文件B (2)将学生信息转化成字符数组存入文本文件A中 (3)使用for循环，if-else语句将诗句按照规定的格式存入文本文件B中 (4)try-catch语句进行异常处理
#核心代码
 Student stu=new Student();
        Scanner sc= new Scanner(System.in);

        System.out.println("输入姓名：");
        name=sc.next();

        System.out.println("输入学号：");
        stuNum=sc.nextInt();

        System.out.println("输入年龄：");
        age=sc.nextInt();

        String str="姓名:"+name+" 学号:"+stuNum+" 年龄:"+age;
        return str;

for (int i=7,x=0; i<=14*17;i+=7,x+=7) { //输出诗句到文件

                if (i % 2 == 0) {
                    for (int j = x; j < i; j++) {
                        out.write(c[j]);
                    }
                    out.write("。\n");

                } else {
                    for (int j = x; j < i; j++) {
                        out.write(c[j]);
                    }
                    out.write(",");
#实验感想
通过对程序的思考和设计，在一定程度上了解异常处理机制及异常的概念，在一定程度上掌握了抛出异常、捕获异常和异常处理的方法和了解自定义异常类的定义和使用方法。但是在编写程序方面仍然需要提升能力，使得程序更加完善。主要学会了文件的读写方法，以及对内容进行处理。在写的过程中遇到了很多问题，无法将文件B内容导入到文件A中，文字乱码等问题，通过询问同学最终依次解决收获颇多。

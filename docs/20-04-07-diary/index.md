# 20/04/07 Diary


## tricks汇总
- linux下的tar命令
    - -f 指定archive文件
    - -z 使用gzip处理archive文件，生成或解压缩.gz文件
    - -x 从archive中还原文件
    - -c 建立新的archive文件
    1. tar -zxvf file.tar.gz   解压缩得到.tar的archive然后还原archive得到file
    2. tar -zcvf file.tar.gz file 打包并用gzip压缩

- linux下的zip命令： 用于压缩文件
    - -r 递归处理指定文件目录
    - -d 从.zip文件中删除指定文件
    - unzip 用于解压缩

- latex多图并排
```
\begin{figure}[H]
\centering  %图片全局居中
\subfigure[name1]{
\label{Fig.sub.1}
\includegraphics[width=0.45\textwidth]{a.pdf}}
\subfigure[name2]{
\label{Fig.sub.2}
\includegraphics[width=0.45\textwidth]{b.pdf}}
\caption{Main name}
\label{Fig.main}
\end{figure}
```

- pandas
    1. 基本数据类型
        - Series: 一维带标签的数组， ndarray-like， dict-like
        - DataFrame: 二维的数据结构，不同的列可能有不同的数据类型，相当于一个spreadsheet
        ```
        In [37]: d = { "one": pd.Series([1.0, 2.0, 3.0], index=["a", "b", "c"]), "two": pd.Series([1.0, 2.0, 3.0, 4.0], index=["a", "b", "c", "d"]),}

        In [38]: df = pd.DataFrame(d)

        In [39]: df
        Out[39]: 
           one  two
        a  1.0  1.0
        b  2.0  2.0
        c  3.0  3.0
        d  NaN  4.0
        ```
    2. 从 .txt等 中读取数据 `pd.read_csv("a.txt", header=None)`
    3. 太杂了，边用边学吧


### 杂记
看到刘尚育大佬的豆瓣日记，写的他去跳蚤市场买了白岩诗社的胸针且偶遇了一位姑娘后来又一起参加沙龙的故事。没有细读，但真的是让人读起来感觉美好，如清风徐来。不知道是自己阅读太少还是懒于思考的缘故，想要用文字记录时想到的只是初高中应试练就的套路。最近记忆力也差了许多，莫非是要学要记的东西太多，感觉确实太多但又都想记住，但又真的努力去记住了么？有些东西，虽然读起来很熟悉，但自己从头开始复述却陌生的很。
> 你我今夜共在香樟下，像草垛在风力寻找火种 --香樟狂想曲

> 豫章故郡，洪都新府，星分翼枕，地接衡庐



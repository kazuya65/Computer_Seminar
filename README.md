# 2018年度コンピューターゼミ（C言語)

以下の2つのアルゴリズムを実装し、4/19日のコンピューターゼミまでにgithubを用いて提出してください。
関数の引数は例として出しているだけなので各々好きな関数の形を使ってください。


## 宿題1

二分法
関数 f(x) = 0 となる x を範囲 [a, b] の中から見つける C の関数


      double bisection(double a, double b, double (\*f)(double))


を作成せよ．

### 問題
f(x)=10x+100
[a,b]=[-20, 100]
を先ほどの関数を用いて計算せよ。

## 宿題2
Power Method
離散時間マルコフ連鎖における状態推移確率行列 P があるとき，x = x P となる定常ベクトル x を
求める関数


    void dtmc_power_method(int n, double　\*x0, double \*P, double \*x)


を作成せよ．Power Method は以下の計算を x が収束するまで行う．
  x = x P
関数 dtmc_power_method の引数 x0 には初期のベクトルをわたし，
引数 x には定常ベクトルがかえる．nは行列・ベクトルの次元数．
また，行列 P は二次元配列でなく一次元の配列で与える．

### 問題

以下の状態遷移確率行列について上記の関数を用いて計算を行う。

<img src="https://latex.codecogs.com/gif.latex?\begin{bmatrix}&space;0.6&space;&&space;0.3&space;&&space;0.1&space;\\&space;0.3&space;&&space;0.6&space;&&space;0.1&space;\\&space;0.2&space;&&space;0.3&space;&&space;0.5&space;\end{bmatrix}" />


x0=(1,0,0)

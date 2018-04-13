#2018年度コンピューターゼミ（C言語)

以下の2つのアルゴリズムを実装し、4/19日のコンピューターゼミまでに提出してください。

宿題
二分法
関数 f(x) = 0 となる x を範囲 [a, b] の中から見つける C の関数
 double bisection(double a, double b, double (*f)(double))
を作成せよ．

Power Method
離散時間マルコフ連鎖における状態推移確率行列 P があるとき，x = x P となる定常ベクトル x を
求める関数
  void dtmc_power_method(int n, double *x0, double *P, double *x)
を作成せよ．Power Method は以下の計算を x が収束するまで行う．
  x = x P
関数 dtmc_power_method の引数 x0 には初期のベクトルをわたし，
引数 x には定常ベクトルがかえる．nは行列・ベクトルの次元数．
また，行列 P は二次元配列でなく一次元の配列で与える．

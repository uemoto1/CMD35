# CMD35 Advanced course: SALMON

* 講習資料の訂正事項、ファイル、補足資料の共有用レポジトリです。
This repository is prepared to share the input/output files and additional documents used in the lectures.

## Linear response calculation:
### Upperbound of the frequency range

* 誘電率スペクトル計算（線形応答計算）のスペクトル領域変更: 
スペクトルを取る範囲を変更したい場合は、`analysis`グループの`nenergy`と`de`を調整する
(Add or change the `nenergy` and `de` parameter in `analysis` group) as below:
```
&analysis
    nenergy=  5000
    de= 3.67493E-04
/
```
* `nenergy` = number of the sampling point for energy(frequency) domain
* `de` = spacing in sampling
* maximal frequency of the spectra = `nenergy` * `de`
* detail is explained in the web documents (https://salmon-tddft.jp/webmanual/current/html/input_keyword_list.html#analysis)

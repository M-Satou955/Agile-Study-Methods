# データとデータ型

ソフトウェアの基本　 → 　「データ」と「関数」

### データ

- プログラマが扱う情報のこと。プログラムが実行されると、必ず何らかのデータが必要になる。
- データは、数値、文字列、真偽値など様々な形式で表現されます。

### 関数

- 関数とは、プログラムが実行する手順や操作のこと。関数は、データを処理するための手続きを定義します。例えば、ある数値を 2 乗する関数や、文字列を大文字に変換する関数などがあります。関数は、プログラムの処理の中心となる要素であり、データを処理するために必要不可欠なものです。

データと関数はソフトウェアに必要不可欠であり、データと関数がうまく組み合わさることで、プログラムはさまざまな処理を行い、目的の機能を実現することができる。

コンピューターの中で処理や保存されるデータは、基本的に「0」「1」の２進数の組み合わせで表される。これはコンピューターが電気的な信号として情報を処理しているため。
画像や文字列などのデータもコンピューター内部では２進数で表現

- コンピューターが処理しやすい＆データの転送、保存が効率的にできる。

データの種類を正しく理解し、適切に処理することが重要。
また、プログラムを作成する際には、データを人間が理解しやすい形で表示するための方法も学ぶ必要あり。

## データ型

データ型とはプログラミングにおいて使用されるデータの種類を表す。プログラミングにおいて使用する情報によって、適切なデータ型を選択する必要あり。

代表的なデータ型

- ブーリアン型（真偽値を表す）
- 整数型（整数を表す）
- 浮動小数点型（小数を表す）
- 文字型（1 文字を表す）
- 文字列型（複数の文字列を表す）

### ブーリアン型

プログラミングでは、処理の結果を true または false として扱うことがよくあります。

- 料金が（支払われた / 支払われていない）
- クレジットカードが（有効 / 無効）
- 画面サイズが 800px （より大きい / 以下）
- ユーザーが（有料ユーザー / 無料ユーザー）
- ユーザーがアンケートに（回答した / 未回答）

### 整数型(integer type)

整数を表現することができるデータ型を整数型（integer type）と呼びます。整数型は英語で integer と表記され、int 型と略記されます。

2 進数と 10 進数を相互に変換することによって、コンピュータで整数を扱うことができる

一般的にテキストエディタ上で整数を記述する場合、通常は 10 進数で記述します。整数は、人間が理解しやすく、テキストファイル内で容易に識別できるためです。

ただし、プログラミングにおいては、整数を 2 進数、8 進数、16 進数などの別の進数で表現することがあります。その場合、プログラマはエディタ上で、各進数に合わせた表記方法で整数を記述します。例えば、2 進数で数値「5」を表現する場合は「0b101」と記述し、16 進数で数値「10」を表現する場合は「0x0A」と記述します。

## 整数型の範囲

- int 型（符号付き整数型）: -2,147,483,648 ～ 2,147,483,647
- 符号なし整数型 （unsigned integer data type）: 0 ～ 4,294,967,295

## 大きな整数

int 型を超える範囲の整数を使用する場合は 64 ビットの長さを超えるデータを扱うことができる long 型を使用

### long 型

- 符号付き(long)
- 符号なし(unsigned long)

int 型が 4 バイト、long 型が 8 バイト

long 型を使用する場合、メモリ使用量が int 型使用時に比べ倍になる。
大きな整数を扱わない時は int 型を選択することが推奨。

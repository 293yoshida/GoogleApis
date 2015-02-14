# GoogleApis
GoogleApis の検証用


## Google Maps API の読み込み<br>
 \<script type="text/javascript" <br>
    src="http://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&sensor=SET_TO_TRUE_OR_FALSE"><br>
 \</script>

script タグ内の URL は、JavaScript ファイルの位置を示しており、このファイルには Google Maps API を使用する上で必要なシンボルと定義がすべて入っています。この script タグは必須です。

key パラメータにはアプリケーションの API キーが含まれています。詳細については、API キーを取得するをご覧ください。このキーは、API V2 で使用されていたキーとは異なります。API コンソールから生成する必要があります。

URL の sensor パラメータは必須です。このアプリケーションがユーザーの位置情報を取得するのにセンサー（GPS など）を使用するかどうかを示します。この例では、パラメータの値を true または false に明示的に設定する必要があることを強調するために、set_to_true_or_false を変数のままにしています。


 ## API の非同期読み込み
 Maps API JavaScript コードは、ページの読み込みの完了後に読み込むか、オンデマンドで読み込むことができます。これを行うには、独自の <script> タグを window.onload イベントへのレスポンスや関数コールに挿入します。さらに、Maps JavaScript API ブートストラップに対し、Maps JavaScript API コードが完全に読み込まれてからアプリケーション コードを実行するように指示する必要があります。そのためには、callback パラメータを使用します。このパラメータは、API の読み込み完了後に実行する関数を引数として受け取ります。

次のコードは、ページが完全に読み込まれてから Maps API を読み込み（window.onload を使用）、ページ内の <script> タグに Maps JavaScript API を書き込むようアプリケーションに指示しています。また、Maps API ブートストラップに callback=initialize を渡すことで、API の読み込みが完了してから initialize() 関数を実行するように、API に指示しています。
 
 
 

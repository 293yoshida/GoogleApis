# GoogleApis
GoogleApis の検証用


## Google Maps API の読み込み<br>
 \<script type="text/javascript" <br>
    src="http://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&sensor=SET_TO_TRUE_OR_FALSE"><br>
 \</script>

script タグ内の URL は、JavaScript ファイルの位置を示しており、このファイルには Google Maps API を使用する上で必要なシンボルと定義がすべて入っています。この script タグは必須です。

key パラメータにはアプリケーションの API キーが含まれています。詳細については、API キーを取得するをご覧ください。このキーは、API V2 で使用されていたキーとは異なります。API コンソールから生成する必要があります。

URL の sensor パラメータは必須です。このアプリケーションがユーザーの位置情報を取得するのにセンサー（GPS など）を使用するかどうかを示します。この例では、パラメータの値を true または false に明示的に設定する必要があることを強調するために、set_to_true_or_false を変数のままにしています。




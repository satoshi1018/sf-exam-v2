# 基本仕様
・Userモデルと別のUserモデルをMembershipモデルを中間テーブルとして関連付けをしていってください。  
・関連付けは下記のようにツリー状になるようにしてください。  
<div>User1</div>  
<div>|------------------</div>
<div>|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|</div> 
<div>User2&emsp;&emsp;&emsp;&emsp;&emsp;User3</div> 
<div>|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;|</div>
<div>|-------- &emsp;&emsp;&emsp;&emsp;|-----------</div>  
<div>|&emsp; &emsp;&emsp;&emsp;|&emsp;&emsp;&emsp; |&emsp;&emsp;&emsp;&emsp;&emsp;|</div>
<div>User4&emsp;User5&emsp;User6&emsp;&emsp;User7</div>

・関連付けの名称は任意でお任せします。  
（ただし、上記の関連付けの実態に即した名前にしてください。follow, follower等は名前として不適なので、実装としてはNGです。）  
・ルーティングは基本的にindex, new, create, show, edit, update, destroyを生成すること。 

# Advance1  
・自分に関連付けられる子要素の数は最大で2個まで。  
・上記をvalidationで検証すること  

# Advance2
・usersのshowアクションで、自分に紐づいたUserがツリー状に表示されるようになること。

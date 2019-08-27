# 레이어 중앙 정렬
### Position: absolute와 margin: auto를 이용한 방법
-	position: absolute를 적용하고 top, right, bottom, left 값에 각각 0을 지정합니다.
-	width와 height에 값을 지정합니다.
-	Margin에 auto값 지정합니다.

### Position: absolute와 margin 음수값을 이용한 방법
-	Position: absolute를 적용하고 top: 50%, left: 50%를 지정합니다.
-	Width와 height에 고정값을 지정합니다.
-	Margin-top과 margin-left에 각각 높이의 절반 값과 너비의 절반 값을 지정합니다.

### Position: absolute와 transform을 이용한 방법
-	Position: absolute를 적용하고 top: 50%, left: 50%를 지정합니다.
-	Transform: translate(-50%, -50%)를 적용합니다.

### 두 개의 inline-block 요소를 이용한 방법
-	Layer 요소에 text-align: center를 적용합니다.
-	Content 요소에 display: inline-block, vertical-align: middle을 적용합니다.
-	Content와 형제인 blank 요소에 display: inline-block, vertical-align: middle을 적용합니다.
-	Vertical-align은 형제 요소의 높이값을 기준으로 정렬하기 때문에 세로 중앙 정렬을 위해 blank 요소가 부모 요소의 높이값을 가질 수 있도록 height: 100%를 지정합니다.
-	또한 inline-block 간에 생기는 4px의 공백을 제거합니다. (margin 음수값, 부모 요소의 font-size: 0 설정 등)

### 두 개의 inline-block 요소 중 Blank 요소를 가상 요소로 대체하는 방법
-	위에서 blank 요소를 사용하는 방법은 필요 없는 요소를 하나 더 사용해야만 합니다. Css로 가상 요소를 생성하여 해당 요소를 대신할 수 있습니다.

### table-cell과 inline-block을 이용한 방법
-	Layer 요소에 display: table을 적용합니다.
-	Inner 요소에 display: table-cell, text-align: center, vertical-align: middle을 적용합니다.
-	Content 요소에 display: inline-block을 적용하여 중앙에 정렬되도록 합니다.

### Table-cell과 margin: 0 auto를 이용한 방법
-	Layer 요소에 display: table을 적용합니다.
-	Inner 요소에 display: table-cell, vertical-align: middle을 적용합니다.
-	Content 요소에 width값을 지정하고 display: block, margin: 0 auto를 적용합니다.

### Flex를 이용한 방법 (IE10 이상)
-	Layer 요소에 display: flex, justify-content: center, align-items: center를 적용하여 content 요소를 중앙 정렬합니다.

### Flex와 margin: auto를 이용한 방법 (IE 사용 불가)
-	Layer 요소에 display: flex를 적용합니다.
-	Content 요소에 maring: auto를 적용합니다.

### Grid (IE 사용 불가)
-	Layer 요소에 display: grid를 적용합니다.
-	Content 요소에 margin: auto를 적용합니다.

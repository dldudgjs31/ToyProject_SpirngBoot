<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>Spring Boot 프로젝트</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	text-indent: -1.7em;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, YuMincho, "Yu Mincho", "Hiragino Mincho ProN", "Hiragino Mincho Pro", "Songti TC", "Songti SC", "SimSun", "Nanum Myeongjo", NanumMyeongjo, Batang, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC', 'Noto Sans CJK KR'; }

.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC', 'Noto Sans Mono CJK KR'; }

.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, YuMincho, "Yu Mincho", "Hiragino Mincho ProN", "Hiragino Mincho Pro", "Songti TC", "Songti SC", "SimSun", "Nanum Myeongjo", NanumMyeongjo, Batang, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC', 'Noto Sans CJK KR'; }

.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC', 'Noto Sans Mono CJK KR'; }

.highlight-default {
}
.highlight-gray {
	color: rgb(155,154,151);
}
.highlight-brown {
	color: rgb(100,71,58);
}
.highlight-orange {
	color: rgb(217,115,13);
}
.highlight-yellow {
	color: rgb(223,171,1);
}
.highlight-teal {
	color: rgb(15,123,108);
}
.highlight-blue {
	color: rgb(11,110,153);
}
.highlight-purple {
	color: rgb(105,64,165);
}
.highlight-pink {
	color: rgb(173,26,114);
}
.highlight-red {
	color: rgb(224,62,62);
}
.highlight-gray_background {
	background: rgb(235,236,237);
}
.highlight-brown_background {
	background: rgb(233,229,227);
}
.highlight-orange_background {
	background: rgb(250,235,221);
}
.highlight-yellow_background {
	background: rgb(251,243,219);
}
.highlight-teal_background {
	background: rgb(221,237,234);
}
.highlight-blue_background {
	background: rgb(221,235,241);
}
.highlight-purple_background {
	background: rgb(234,228,242);
}
.highlight-pink_background {
	background: rgb(244,223,235);
}
.highlight-red_background {
	background: rgb(251,228,228);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(55, 53, 47, 0.6);
	fill: rgba(55, 53, 47, 0.6);
}
.block-color-brown {
	color: rgb(100,71,58);
	fill: rgb(100,71,58);
}
.block-color-orange {
	color: rgb(217,115,13);
	fill: rgb(217,115,13);
}
.block-color-yellow {
	color: rgb(223,171,1);
	fill: rgb(223,171,1);
}
.block-color-teal {
	color: rgb(15,123,108);
	fill: rgb(15,123,108);
}
.block-color-blue {
	color: rgb(11,110,153);
	fill: rgb(11,110,153);
}
.block-color-purple {
	color: rgb(105,64,165);
	fill: rgb(105,64,165);
}
.block-color-pink {
	color: rgb(173,26,114);
	fill: rgb(173,26,114);
}
.block-color-red {
	color: rgb(224,62,62);
	fill: rgb(224,62,62);
}
.block-color-gray_background {
	background: rgb(235,236,237);
}
.block-color-brown_background {
	background: rgb(233,229,227);
}
.block-color-orange_background {
	background: rgb(250,235,221);
}
.block-color-yellow_background {
	background: rgb(251,243,219);
}
.block-color-teal_background {
	background: rgb(221,237,234);
}
.block-color-blue_background {
	background: rgb(221,235,241);
}
.block-color-purple_background {
	background: rgb(234,228,242);
}
.block-color-pink_background {
	background: rgb(244,223,235);
}
.block-color-red_background {
	background: rgb(251,228,228);
}
.select-value-color-default { background-color: rgba(206,205,202,0.5); }
.select-value-color-gray { background-color: rgba(155,154,151, 0.4); }
.select-value-color-brown { background-color: rgba(140,46,0,0.2); }
.select-value-color-orange { background-color: rgba(245,93,0,0.2); }
.select-value-color-yellow { background-color: rgba(233,168,0,0.2); }
.select-value-color-green { background-color: rgba(0,135,107,0.2); }
.select-value-color-blue { background-color: rgba(0,120,223,0.2); }
.select-value-color-purple { background-color: rgba(103,36,222,0.2); }
.select-value-color-pink { background-color: rgba(221,0,129,0.2); }
.select-value-color-red { background-color: rgba(255,0,26,0.2); }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="58647b1b-5c80-45c0-839f-a18189e1df7b" class="page sans"><header><div class="page-header-icon undefined"><span class="icon">🍃</span></div><h1 class="page-title">Spring Boot 프로젝트</h1></header><div class="page-body"><p id="042b2d85-9e0f-4429-ad14-f72bfe76e297" class="">멤버 : 이영헌, 전상훈</p><h3 id="b6761436-c114-4b01-b9e9-b7002293397b" class="">프로젝트 개요</h3><p id="f55c8a7d-7784-4fcc-8d53-c0c6c61717db" class="">개발환경: Spring Boot (version 2.5.2)</p><p id="e9e9c05e-069a-45c9-8cea-4e81c4c6aec2" class="">언어 : Java 1.8</p><p id="01756322-9747-4e9d-8939-8950b09b03db" class="">빌드툴 : Gradle</p><p id="5e9ba396-6aa2-4a11-a2e7-7df6da6854a5" class="">배포 패키징 : War</p><p id="e7fb1ed6-f501-4435-ab78-7f25e1ab27ba" class="">DB : OracleDB / myBatis</p><p id="d835a774-ce3e-478e-8e01-6212b578fcc1" class="">뷰 : JSP</p><p id="24e79d42-1017-4125-bae3-ba1ade7b1fd7" class="">WEB-WAS : Tomcat (추후 Jboss/Apache)</p><p id="d80283c7-0420-43f9-8ddc-402d524dbebb" class="">형상 관리 : Git / Github</p><h3 id="9be85f31-df77-41a6-8127-aa0e500e758a" class="">프로젝트 목표</h3><ol id="eadbc956-6a08-45d7-ad59-9fd4fa70d79a" class="numbered-list" start="1"><li>Spring boot 기능 스터디</li></ol><ol id="0c62295d-7ac1-4d3c-948c-4bc2e2e7bf18" class="numbered-list" start="2"><li>Spring boot 환경 설정 (Logging, DB 등)</li></ol><ol id="d0099f7c-2762-44e8-b89f-ed338d2d56f3" class="numbered-list" start="3"><li>외부 라이브러리 사용 (부트스트랩 등)</li></ol><ol id="e907668e-ada2-4815-8f72-c3de2eeb98df" class="numbered-list" start="4"><li>DB 프레임워크 사용</li></ol><ol id="efc4a34f-5505-48e4-bbc2-713834faca1d" class="numbered-list" start="5"><li>공공 API / 기타 API 사용 (지도, 날씨 등)</li></ol><ol id="33aeba61-a54d-474f-9f8a-1f257f16bf94" class="numbered-list" start="6"><li>로그인 기능 구현 (타 SNS 계정 연동)</li></ol><ol id="5add0cbd-52d9-42b6-8d36-dc263573758f" class="numbered-list" start="7"><li>채팅 기능 구현</li></ol><ol id="3d491fea-bebb-4f2d-b6b7-a49739ac9132" class="numbered-list" start="8"><li>Spring MVC 구조 파악</li></ol><ol id="0b8f4ed0-7861-4a8d-b120-eec6a56aa13a" class="numbered-list" start="9"><li>오픈소스 WEB-WAS 배포 진행<figure id="eeac14d2-b587-480d-9ac5-ea4ffe5e6e00"><a href="https://github.com/dldudgjs31/ToyProject_SpirngBoot" class="bookmark source"><div class="bookmark-info"><div class="bookmark-text"><div class="bookmark-title">dldudgjs31/ToyProject_SpirngBoot</div><div class="bookmark-description">ToyProject_SpirngBoot. Contribute to dldudgjs31/ToyProject_SpirngBoot development by creating an account on GitHub.</div></div><div class="bookmark-href"><img src="https://github.com/favicon.ico" class="icon bookmark-icon"/>https://github.com/dldudgjs31/ToyProject_SpirngBoot</div></div><img src="https://opengraph.githubassets.com/263757fcf73f17d03de17bf406414343c009fc1aae62a5770047d46afaec34c3/dldudgjs31/ToyProject_SpirngBoot" class="bookmark-image"/></a></figure></li></ol><p id="44e67bda-ba7c-4254-8dfe-04b00b5dd8f7" class="">
</p><h3 id="0dd5dab9-2382-4ecc-9588-45e869192183" class="">프로젝트 주제</h3><p id="8335d09f-26f4-44d4-8ef8-c46856083790" class="">패션에 대한 리뷰 / 의견 공유 커뮤니티..</p><h3 id="4292212e-7976-4539-8537-66729fcfc795" class="">프로젝트 요구사항</h3><ol id="a28a1147-8ce0-481c-9ac7-a78964a2cff2" class="numbered-list" start="1"><li>일반 회원</li></ol><ul id="84c2c6cb-1468-4f9a-a632-1777a5a9e54a" class="bulleted-list"><li>회원가입 (1인 1계정 주민번호/핸드폰 번호당 1개)</li></ul><ul id="4acc7c09-8aef-419a-8374-160d0107d2f6" class="bulleted-list"><li>회원가입 본인의 프로필을 등록할 수 있다.(사진 등)</li></ul><ul id="72f379fc-702b-4445-8dba-731f2c22c402" class="bulleted-list"><li>회원들은 닉네임 사용(중복 체크), (월 1회 변경 가능)</li></ul><ul id="cb9c2577-345d-4d66-97e6-005ebaea7148" class="bulleted-list"><li>회원 가입시 위치 등록(주소)</li></ul><ul id="e3fd0e73-d158-4eaa-8ff1-8cad6c7b548a" class="bulleted-list"><li>회원가입시 타sns 계정 연동이 가능하다.(카카오/네이버)</li></ul><ul id="c024a4a9-681f-40a8-9c73-3ecf9f630199" class="bulleted-list"><li>게시글을 볼 수 있는 mypage가 있다. (활동내역 확인가능 / 커뮤니티, 스토어)</li></ul><ul id="aac4b94f-35bc-4fed-98b7-8ca719e6e977" class="bulleted-list"><li>비밀번호 변경시 과거 사용 번호 사용 불가(5개까지)</li></ul><ul id="3715cdb5-e5b9-4787-9d2a-d1aec682abb5" class="bulleted-list"><li>각 회원은 등급을 가지고 있다.(게시한 글(인기글 등록시),로그인 시 쌓이는 방식)</li></ul><ul id="4f182dd3-85bb-4721-9bdc-634c70e1200d" class="bulleted-list"><li>관심 브랜드들을 즐겨찾기 할 수 있다.</li></ul><p id="43fe7ec8-b73c-44f8-ba3d-6d0d69e57c0e" class="">
</p><p id="2164660d-7dba-4ea2-8710-6893f21c5459" class="">게시판</p><ul id="fab6b277-1e7c-4aa3-af5e-602879f2c89a" class="bulleted-list"><li>패션점검 게시판에 글을 올릴 수 있다.</li></ul><ul id="8563843a-4687-4ceb-ac70-c972b8f84a59" class="bulleted-list"><li>OOTD 게시판 글을 올릴 수 있다.(본인 패션 스타일 기재, 관련 제품 태그)(이주의 HOT패션 (추천수 기준))(중고게시판과 연동)</li></ul><ul id="79184373-21d0-44a6-af93-844161e2daab" class="bulleted-list"><li>자유 게시판에 글을 올릴 수 있다. (이주의 HOT 게시글(추천수 기준))</li></ul><ul id="9ff40031-a069-4d7d-a16e-79402528c352" class="bulleted-list"><li>패션테러리스트 게시판( 최악의 패션을 공유 )(아이디 익명으로 노출)</li></ul><ul id="7e6f146c-cdaa-4241-b1ad-88d5dbeab2cb" class="bulleted-list"><li>입점 브랜드 리뷰 게시판 (잡플래닛 느낌)</li></ul><ul id="4af3e82d-7a40-4661-bbfe-fc4c8e207de8" class="bulleted-list"><li>Q&amp;A 게시판</li></ul><ul id="be29a896-e7ad-4475-b65b-d7784816dc8e" class="bulleted-list"><li>자유 실시간 채팅</li></ul><ul id="1e16c8ac-c9f2-464f-95e3-c90a60e9a9f3" class="bulleted-list"><li>IT아이템 월드컵(알고리즘 짜면 재밋을듯 ㅅㅂ)</li></ul><ul id="d01b63b5-1182-4671-a0cc-d41f11ad81a6" class="bulleted-list"><li>오프라인 매장 확인하기 게시판 (판매자가 위치등록한 DB 사용)</li></ul><ul id="f5e3395f-6b98-40d3-a650-6b4d41c0a94e" class="bulleted-list"><li>중고거래 게시판( 지도API )(당근마켓)</li></ul><p id="a7fdae23-19b5-4aef-8f70-5e19e83126a1" class="">
</p><p id="5589e7bc-e1d9-423e-9c69-8ac521d50ae6" class="">2. 스토어 (보류)</p><ol id="75bf0b8c-e38c-452c-8a85-9ef667688649" class="numbered-list" start="1"><li>제품 디테일 (이미지 등록)</li></ol><ol id="ad27de3d-3c88-43b1-88bc-693d365986c1" class="numbered-list" start="2"><li>Q&amp;A 게시판</li></ol><ol id="c4152a29-165e-41a8-95fe-11d23bb654c7" class="numbered-list" start="3"><li>리뷰 게시판</li></ol><ol id="f92d298f-b6b6-441d-85c5-8d6b9ad28140" class="numbered-list" start="4"><li>결제수단 선택(카카오 페이,네이버 페이 등등)</li></ol><ol id="196e8d9d-6848-4d3d-9c30-9b28e0a40d01" class="numbered-list" start="5"><li>검색 필터 기능</li></ol><p id="1148d2ba-ed4b-4a58-b663-7ed694bffe24" class="">
</p><p id="8a93b10e-42d7-45dc-bf7b-bb150399a7ef" class="">3. 관리자</p><ul id="869fba53-632b-4892-9302-e034b84cddc1" class="bulleted-list"><li>공지사항 게시판</li></ul><ul id="8b5f993a-ae33-4c28-817f-f69a4f775d10" class="bulleted-list"><li>이벤트 게시판</li></ul><ul id="c3e2ea35-7ce6-46be-8de3-2a2866ef5548" class="bulleted-list"><li>DASHBOARD (마지막)</li></ul><h3 id="4a0a9e54-c5f5-4584-aa83-ad6c5a927738" class="">DB 설계</h3><figure id="579e43d2-ff2f-4355-bd80-888fe90de4c1"><a href="https://www.erdcloud.com/d/ayRa9fNqcH4KyH5Km" class="bookmark source"><div class="bookmark-info"><div class="bookmark-text"><div class="bookmark-title">TEST</div><div class="bookmark-description">Draw ERD with your team members. All states are shared in real time. And it&#x27;s FREE. Database modeling tool.</div></div><div class="bookmark-href"><img src="https://www.erdcloud.com/favicon-16x16.png" class="icon bookmark-icon"/>https://www.erdcloud.com/d/ayRa9fNqcH4KyH5Km</div></div></a></figure><h3 id="6688e471-d414-469e-af51-2a216003ef4f" class="">화면 UI 설계</h3><p id="6ceceef8-8e83-4be3-b258-fe0f581d45f6" class="">
</p><p id="d58c2162-215a-46ae-80ce-57d5e3b42d21" class="">
</p><figure id="1a006e5c-8ee4-4ca3-a5f0-d4b59f2d200c" class="image"><a href="Spring%20Boot%20%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3%201a006e5c8ee44ca3a5f0d4b59f2d200c/Untitled.png"><img style="width:1170px" src="Spring%20Boot%20%E1%84%91%E1%85%B3%E1%84%85%E1%85%A9%E1%84%8C%E1%85%A6%E1%86%A8%E1%84%90%E1%85%B3%201a006e5c8ee44ca3a5f0d4b59f2d200c/Untitled.png"/></a></figure><p id="d34ae8ca-bbd2-4460-9d69-3f71d645885a" class="">
</p></div></article></body></html>

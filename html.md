HTML (Hyper Text Markup Language)      


1. 기본구조 
<HTML>
 <HEAD>
   <TITLE>문서의 제목</TITLE>
  </HEAD>
<BODY>
 내용
</BODY>
</HTML> 

 

<Hn></Hn>       표제 부분에 들어갈 말을 정의. 1~6까지의 숫자를 사용하고 숫자가 커질수록 표제는 작아짐 default H4
<!--주석-->    주석을 달거나 잠시 이미지를 보이지 않게 할때 사용

 

 

2. 문단 혹은 줄을 바꾸는 태그
&nbsp;                            공백
<P align="">                     문단을 바꾸는 태그 줄바꿈과 동시에 줄을 띈 것같은 효과
<BR>                               문단을 바꾸는 태그 줄바꿈의 역할만 수행
<PRE></PRE>                      여백이나 줄간격 등을 고정시켜 주는 역할
<BLOCKQUOTE></BLOCKQUOTE>  들여쓰기
<CNETER></CENTER>              전체 문장을 가운데로 정렬
- align : 정렬하기 (left/center/right)

 


3. 글자관련 태그
<FONT size="n" face="글꼴" color="색깔"></FONT> 
- size : 글자의 크기를 마음대로 조절. 숫자는 1~7까지며 7이 가장 큰 크기 (default : 3)

 

<STRONG></STRONG> , <B></B>                 굵은 글씨를 나타내 주는 태그
<I></I>, <EM></EM>, <VAR></VAR>             이탤릭체의 글씨를 나타내 주는 태그
<KBD></KBD>, <CODE></CODE>, <TT></TT>     타자기체의 글씨를 나타내 주는 태그
<U></U>                                            글자에 밑줄
<S></S>                                            글자 중앙을 가로지르는 중앙선을 긋는 태그
<BIG></BIG>                                      글자 크기를 크게 변경
<SMALL></SMALL>                               글자 크기를 작게 변경    
<BLINK></BLINK>                                 글자를 깜박이게

<SUB></SUB>                                      아랫첨자
<SUP></SUP>                                      윗첨자

 


4. 선 그리기 태그
<HR align="" width="" size="">   입체적인 선을 그려줌 
- align : 선의 정렬 
- width : 선의 폭 
- size : 선의 높이

 


5. 목록을 정리해 주는 태그
<UL></UL>    순서가 없는 목록. 일반적인 나열
<OL></OL>      순서가 있는 목록. 위에서부터 번호 매김
<MENU></MENU>   메뉴 목록으로 그리길지 않은 문장의 열거에 사용
<DIR></DIR>        디렉토리 목록으로 메뉴 목록보다 짧은 문장을 나열
<DL></DL>          정의 목록 태그 <LI>가 아닌<DT>와 <DD>를 사용

 


6. 하이퍼링크
<A href="URL"></A>    다른 홈페이지와 연결
<A name=""></A>       자신의 홈페이지 내에서 연결 (책갈피) (다른 페이지에서 책갈피로드 : URL#name)
<A href="URL" target="_self/_blank">
- href : 연결될 URL 지정 ("mailto:mail-address" : 메일보내기)
- target
 _self : 지금 창에서 연결 (default)
 _blank : 새창으로 연결
 
 
7. 배경 이미지, 색상 지정
<BODY background="이미지경로">      배경 이미지 띄어줌
<BODY bgcolor="색깔">                 배경 색깔을 지정
<BODY text="#nnnnnn"></BODY>      글자색을 지정
<BODY link="#nnnnnn"></BODY>        하이퍼링크의 색을 지정
<BODY vlink="#nnnnnn"></BODY>      한번 누른적이 있는 하이퍼링크의 색을 지정
<BODY alink="#nnnnnn"></BODY>      누르고 있는 동안의 하이퍼링크의 색을 지정

 

* 색상
#00000000
보통 6자리로 색상을 표현하는데 가끔 8자리인경우가 있다.
이때 8자리에서 앞 두자리는 알파값 즉, 투명도를 나타낸다. (00 : 투명 ~ ff : 불투명 )

 


8. 표 만들기 태그
<TABLE width="" height="" border="" bordercolor="테두리 색깔" background="" frame="" rules="" cellspacing="" cellpadding="" align="">      
<TR>
 <TD>1행 1열</TD>
 <TD>1행 2열</TD>
</TR>  
<TR>
 <TD>2행 1열</TD>
 <TD>2행 2열</TD>
</TR>  
</TABLE>     

- background : 테이블 배경 이미지 지정
- frame : 바깥쪽 테두리 (void / boxs)
- rules : 안쪽 테두리 (none : 테두리 없음 / cols : 열사이만 테두리 / rows : 행사이만 테두리)
- cellspacing : 셀간의 여백 지정
- cellpadding : 셀과 내용물간의 여백 지정
- align : 테이블 정렬 (left / center / right)

 

<TD bgcolor="" colspan="" rowspan="" align="" valign="" nowrap>    
- colspan : 가로칸을 n만큼 병합
- rowspan : 세로칸을 n만큼 병합
- align : 표안의 좌우 정렬 방식을 정의 
- valign : 표안의 상하 정렬 방식을 정의 (top / middle / bottom)
- nowrap : 셀 줄바꿈 안되게 지정


<TH>        제목줄    

 


9. 흐르는 글자 태그
<MARQUEE width="" height="" bgcolor="색깔" behavior="alternate/slide" direction="up/right/..." loop="" scrollmount="" scrolldelay=""> </MARQUEE>
- width, height : 크기 지정
- bgcolor : 배경 색깔
- behavior 
 alternate : 좌우로 왔다 갔다함
 slide : 움직이다가 멈춤
- direction : 방향 지정  
- loop : 움직이는 횟수 지정
- scrollmount : 움직이게 되는 길이를 픽셀단위로 지정
- scrolldelay : 움직일 속도를 지정

 


10. 이미지 태그
<IMG src="이미지 경로" width="n" height="n" border=n vspace="n" hspace="n" align="left/right/..." alt="설명">
- src : 이미지 경로
- width, height : 이미지 크기 지정
- border : 이미지 테두리 굵기 지정
- vspace, hspace : 좌우, 상하 여백 지정
- align : 정렬 (middle : 이미지의 세로 중앙에 글 문단이 정렬)
- alt : 말풍선

 


11. 이미지 맵
<IMG src="이미지 경로" usemap="#menu>
<MAP name="menu">
<AREA shape="rect/circle/poly" coords="좌표" href="URL" alt="설명">
</MAP>
- name : <IMG> 의 usemap 에서 지정한 맵이름과 동일해야한다.
- shape : 이미지맵의 모양을 사각형(rect), 타원형(circle), 다각형(poly) 중에 지정
- coords : shape 에서 선택한 이미지맵에 따라 좌표부분이 달라진다. 다각형의 경우 최소 3개의 꼭지점이 필요하다. 
             (circle : 중심점 x좌표, 중심점 y좌표, 반지름)
 
 
12. 음악 태그
<BGSOUND src="음악파일 경로" loop="">
<EMBED src="음악파일 경로" autostart="true/false" hidden="true/false" loop="true/false/">
 - autostart : 자동 시작 설정
 - loop : 반복여부 설정 (-1 : 무한반복)

 


13. FORM
<FORM>
<INPUT type="text" name="" value="" size="" maxlength="">         텍스트 입력창
<INPUT type="password" name="" value="" size="" maxlength="">   패스워드 입력창
<TEXTAREA name="" rows="" cols=""> </TEXTAREA>                       텍스트 영역
<INPUT type="radio" name="" value="" checked>                          라디오버튼
<INPUT type="checkbox" name="" value="" checked>                     체크박스
<SELECT name="">                                                                 콤보박스
 <OPTION value=""> </OPTION>
 <OPTION value="" selected> </OPTION>
 ...
</SELECT>
<INPUT type="file" name="" size="">                                         파일 선택 상자
<INPUT type="submit" name="" value="">                                   전송버튼
<INPUT type="reset" name="" value="">                                     취소버튼
<INPUT type="image" name="" src="이미지 경로" alt="설명" align=""> 이미지 버튼
</FORM>

 

 

14. 프레임

<FRAMESET cols/rows="" border="" bordercolor="" frameborder="yes/no" framespacing="">
  <FRAME name="프레임 이름" src="프레임 문서 경로" marginheight="" marginwidth="" scrolling="auto/yes/no" noresize>
  </FRAME>
</FRMAMSET>
- cols : 프레임을 세로방향으로 나누며 가로 폭의 넓이 값을 픽셀이나 퍼센트 단위로 지정
- rows : 프레임을 가로방향으로 나누며 세로 높이의 넓이 값을 픽셀이나 퍼센트 단위로 지정
- border : 프레임 테두리 굵기 지정
- fameborder : yes, no 로 지정하면 프레임 테두리를 화면에 보이게 하거나 없어지게 한다.
- framespacing : 여백 크기 지정
 


* 프레임 문서에서의 하이퍼 타깃
<A href="파일 경로" target="프레임 이름/_top/_self_/_blank/_parent"> 내용... </A>
- target 
   1. 프레임 이름 : <FRAME> 태그의 name 속성에서 지정한 프레임 이름을 타깃으로 지정하면 지정한 프레임에 하이퍼링크 문서가 나타난다.
   2. _top : 프레임 구조를 무시하고 전체화면 창으로 하이퍼링크 문서가 나타난다.
   3. _self : 기본값으로 현재 프레임 화면에 하이퍼링크 문서가 나타난다.
   4. _blank : 새로운 화면에 하이퍼링크 문서가 나타난다.
   5. _parent : 프레임의 상위 프레임 세트에 하이퍼링크 문서가 나타난다. 복잡한 프레임 세트 구조에서 확인할수있다.
 


15. 그 밖의 태그들
<DFN></DFN>                        정의되어지는 단어에 대한 것
<CITE></CITE>                      책이나 사진 등의 제목
<SAMP></SAMP>                  컴퓨터상에 메세지
<BASEPOINT>...</BASEPOINT>  기본적으로 미리 약속된 크기를 다시 정할때 사용

PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> pwd

Path
----
C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo


PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> ls


    디렉터리: C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-03-20   오후 2:20                venv
-a----      2026-03-20   오후 2:48            270 .gitignore
-a----      2026-03-20   오후 2:30           1064 app.py
-a----      2026-03-20   오후 2:23           1772 requirements.txt


PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> cd venv
PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo\venv> cd ..
PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> mkdir 3week


    디렉터리: C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-03-20   오후 4:00                3week


PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> cat app.py
import streamlit as st 
import pandas as pd
# ?섏씠吏 ?ㅼ젙
st.set_page_config(page_title="鍮낅뜲?댄꽣 遺꾩꽍 ?꾨줈?앺듃", page_icon="?뱤")
# ?쒕ぉ
st.title("鍮낅뜲?댄꽣 遺꾩꽍 ?꾨줈?앺듃")
st.write("泥?踰덉㎏ Streamlit ?깆엯?덈떎!")
# 援щ텇??
st.divider()
# 媛꾨떒??李⑦듃
st.subheader("Python ?먯닔 李⑦듃")

# 媛꾨떒???곗씠?고봽?덉엫 ?쒖떆
st.subheader("?섑뵆 ?곗씠??)
data = {
"?대쫫": ["源泥좎닔", "?댁쁺??, "諛뺣???, "?뺤닔吏?, "理쒖???],
"?숇뀈": [3, 3, 3, 3, 3],
"?꾧났": ["AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??],
"Python?먯닔": [85, 92, 78, 95, 88]
}
df = pd.DataFrame(data)
st.dataframe(df, use_container_width=True)
st.bar_chart(df.set_index("?대쫫")["Python?먯닔"])
# ?ъ씠?쒕컮
st.sidebar.header("?ㅼ젙") 
st.sidebar.write("???곸뿭? ?ъ씠?쒕컮?낅땲??")
name = st.sidebar.text_input("?대쫫???낅젰?섏꽭??)
if name:
    st.sidebar.write(f"?덈뀞?섏꽭?? {name}??")
PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> cp app.py
cp : C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo\app.py 항목을 자기 자신으로 덮어쓸 수 없습니다.
위치 줄:1 문자:1
+ cp app.py
+ ~~~~~~~~~
    + CategoryInfo          : WriteError: (C:\sunwoo\과제\빅데...b-sunwoo\app.py:String) [Copy-Item], IOException
    + FullyQualifiedErrorId : CopyError,Microsoft.PowerShell.Commands.CopyItemCommand

PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> cp .gitignore
cp : C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo\.gitignore 항목을 자기 자신으로 덮어쓸 수 없습니다.
위치 줄:1 문자:1
+ cp .gitignore
+ ~~~~~~~~~~~~~
    + CategoryInfo          : WriteError: (C:\sunwoo\과제\빅데...nwoo\.gitignore:String) [Copy-Item], IOException
    + FullyQualifiedErrorId : CopyError,Microsoft.PowerShell.Commands.CopyItemCommand

PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> mkdir abc.py 


    디렉터리: C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-03-20   오후 4:02                abc.py


PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> cp app.py .gitignore
PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> mv app.py application.py
PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> rm abc.py
rm : 'C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo\abc.py' 경로는 존재하지 않으므로 찾을 수 없습니다.
위치 줄:1 문자:1
+ rm abc.py
+ ~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\sunwoo\과제\빅데...b-sunwoo\abc.py:String) [Remove-Item], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.RemoveItemCommand

PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> rm abc.py
PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> rm -3week
rm : 'C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo\-3week' 경로는 존재하지 않으므로 찾을 수 없습니다.
위치 줄:1 문자:1
+ rm -3week
+ ~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\sunwoo\과제\빅데...b-sunwoo\-3week:String) [Remove-Item], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Commands.RemoveItemCommand

PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> rm -Recurse 3week
PS C:\sunwoo\과제\빅데이터분석 프로그래밍\bigdata-project-b-sunwoo> 
import streamlit as st

st.set_page_config(page_title="시끄러움 지수", page_icon="🔊")

st.title("🔊 반 시끄러움 지수")

# 슬라이더
noise = st.slider("현재 시끄러움 정도", 0, 100, 50)

# 색상 판별
if noise < 40:
    color = "🟢 초록"
    message = "조용해요!"
elif noise < 70:
    color = "🟠 주황"
    message = "조금 시끄러워요!"
else:
    color = "🔴 빨강"
    message = "너무 시끄러워요!"

# 결과 출력
st.subheader(f"현재 상태: {color}")
st.write(message)

# 진행 바
st.progress(noise)

import streamlit as st

if "score" not in st.session_state:
    st.session_state.score = 0
if "per_click" not in st.session_state:
    st.session_state.per_click = 1
st.title("Clicker Game")
st.write(f"Score: {st.session_state.score}")
st.write(f"Points per Click: {st.session_state.per_click}")

if st.button("Click me!"):
    st.session_state.score += st.session_state.per_click
if st.button("Upgrade (Cost: 5 points)"):
    if st.session_state.score >= 5:
        st.session_state.score -= 5
        st.session_state.per_click += 1
    else:
        st.write("Not enough points")

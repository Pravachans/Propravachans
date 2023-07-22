from PIL import Image
import requests
import streamlit as st



st.set_page_config(page_title="My Webpage", page_icon=":tada:", layout="wide")

def load_lottieurl(url):
    r = requests.get(url)
    if r.status_code != 200:
        return None
    return r.json()



# ---- LOAD ASSETS ----
lottie_coding = load_lottieurl("https://assets3.lottiefiles.com/packages/lf20_3fuksula.json")



# ---- HEADER SECTION ----
with st.container():
    st.subheader("Hi, I am Pravachan :wave:")
    st.title("A Youtuber from Netherlands")
    st.write("I am proud for the subscribers I have and I tell about my travel, how I live, show my friendly friends and what I do in my house and outside.")


# ---- WHAT I DO ----
with st.container():
    st.write("---")
    left_column, right_column = st.columns(2)
    with left_column:
        st.header("What I do")
        st.write("##")
        st.write(
            """
            On My Youtube Channel I am creating videos for people who:
            - are kind and likes my videos all day long
            - are finding something to watch
            - want to subscribe a Channel
            - watch travel videos

            If you this sounds intresting to you, consider subscribing and turning on the notifications and like.
            """
        )
        st.markdown("[YOUTUBE CHANNEL](https://www.youtube.com/@propravachan6754)")

    with right_column:
        st_lottie(lottie_coding, height=300, key="coding")

# ---- PROJECTS ----
with st.container():
    st.write("---")
    st.header("My Projects")
    st.write("##")
    image_column, text_column = st.columns((1, 2))

        # insert image
with text_column:
        st.subheader("Me playing Fortnite")
        st.write(
            """
            Watch how I play Fortnite, realise how hard is it to play Fortnite.
            Learn the basics of Fortnite.
            See how bad I am or good I am.
            """
        )
        st.markdown("[Watch Video...](https://www.youtube.com/watch?v=xH8yfQJEa50&t=715s)")
with st.container():


    with text_column:
        st.subheader("Tour for Google Sites")
        st.write(
        """
        Want to learn how to use Google Sites?
        Look at this video to learn about it.
        """

    )
    st.markdown("[Watch Video...](https://www.youtube.com/watch?v=UXl0Jb89ahU&t=124s)")

# ----CONTACT ----
with st.container():
    st.write("---")
    st.header("Get In Touch With Me")
    st.write("##")


    contact_form = """
    <form action="https://formsubmit.co/propravachan@gmail.com" method="POST">
        <input type="hidden" name="_captcha" value="false">
        <input type="text" name="name" placeholder="Your name" required>
        <input type="email" name="email" placeholder="Your email" required>
        <textarea name="message" placeholder="Your message here" required></textarea
        <button type="submit">Send</button>
    </form>
    """
    left_column, right_column = st.columns(2)
    with left_column:
        st.markdown(contact_form, unsafe_allow_html=True)
    with right_column:
            st.empty()

<template>
  <div class="app" id="app">
    <AppHeader/>
    <AppInfo/>
    <AppApart/>
    <AppForm/>
    <AppVideo/>
    <AppMap/>
    <AppQuestions/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader";
import AppInfo from "@/components/AppInfo";
import AppApart from "@/components/AppApart";
import AppForm from "@/components/AppForm";
import AppVideo from "@/components/AppVideo";
import AppMap from "@/components/AppMap";
import AppQuestions from "@/components/AppQuestions";
import AppFooter from "@/components/AppFooter";


export default {
  name: 'App',
  components: {
    AppHeader,
    AppInfo,
    AppApart,
    AppForm,
    AppVideo,
    AppMap,
    AppQuestions,
    AppFooter
  }
}
</script>

<style>
.app
html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  color: #fff;
  vertical-align: baseline;
}

ol,
ul,
h1,
h2,
h3,
a {
  list-style: none;
  text-decoration: none;
}

h2 {
  font-family: 'Playfair Display';
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  line-height: 48px;
  color: #D4C17F;
}

@font-face {
  font-family: 'Post No Bills Jaffna SemiBold Regular';
  font-style: normal;
  font-weight: 600;
  src: local('Post No Bills Jaffna SemiBold Regular'), url('./assets/fonts/PostNoBillsJaffna-SemiBold.woff') format('woff');
}

@font-face {
  font-family: 'Raleway';
  src: url('./assets/fonts/Raleway-Regular.woff2') format('woff2'), url('./assets/fonts/Raleway-Regular.woff') format('woff');
  font-weight: 400;
  font-style: normal;
}

@font-face {
  font-family: 'Playfair Display';
  src: url('./assets/fonts/PlayfairDisplay-Bold.woff2') format('woff2'), url('./assets/fonts/PlayfairDisplay-Bold.woff') format('woff');
  font-weight: 700;
  font-style: normal;
}

.wrapper {
  max-width: 1110px;
  margin: 0 auto;
  padding: 0 10px;
}

.background {
  background-color: #242B33;
}

.title {
  font-family: 'Playfair Display';
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  padding-top: 180px;
  color: #D4C17F;
}

.btn {
  display: inline-block;
  line-height: 1;
  font-weight: 700;
  width: 97%;
  border: none;
  padding: 17px;
  transition: all .09s ease-out;
}

.btn-accent {
  background-color: #D4C17F;
  color: #fff;
}

.btn-accent:hover {
  background-color: #907c38;
  color: #fff;
}
.logo{
  font-family: 'Post No Bills Jaffna SemiBold Regular',serif;
  font-size: 17.5px;
  line-height: 0.5;
}
.logo h3{
  font-family: 'Raleway';
  font-size: 12px;
  line-height: 14px;
  letter-spacing: 0.12em;
  margin-top: 5px;
}

</style>

<template>
  <div class="app" id="app">
    <AppHeader/>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader";


export default {
  name: 'App',
  components: {
    AppHeader
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
video{
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
a{
  list-style: none;
  text-decoration: none;
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

.wrapper{
  max-width: 1090px;
  margin: 0 auto;
  padding: 0 10px;
}



</style>

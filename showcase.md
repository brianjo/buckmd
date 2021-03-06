/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.showcase} /\*\* \* Useful for companies with multiple applications.
\* \@param name The name of the project/company that should be
displayed. \* \@param items Items to be displayed for the company. \*
\@param? moreInfo Optional map of titles and a link for more
information. \*/ {template .company}

::: companyShowcase
## {\$name}

{if isNonnull(\$moreInfo)} {foreach \$info in keys(\$moreInfo)}

<div>

[{\$info}](%7B$moreInfo%5B$info%5D%7D){target="_blank"}

</div>

{/foreach} {/if}
:::

{/template} /\*\* \* \@param name The name of the project/company that
should be displayed. \* \@param imgSrc The URL for the image that should
be displayed. \* \@param? links Optional map of titles and a link to the
project/app. \*/ {template .item}

<div>

![{\$name} Logo](%7B$imgSrc%7D)

</div>

<div>

{\$name}

</div>

{if isNonnull(\$links)}

<div>

{foreach \$info in keys(\$links)} {if not isFirst(\$info)} {sp}·{sp}
{/if} [{\$info}](%7B$links%5B$info%5D%7D){target="_blank"} {/foreach}

</div>

{/if}

{/template} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'Showcase\' /} {param navid: \'about_showcase\' /} {param description}
Companies and projects using Buck. {/param} {param content} {call
.company} {param name: \'Facebook\' /} {param moreInfo: quoteKeysIfJs(\[
\'How we build Android apps at Facebook\':
\'https://code.facebook.com/posts/204818946346893/buck-how-we-build-android-apps-at-facebook/\',
\'Amazingly Fast iOS Builds\':
\'https://www.facebook.com/buckbuildtool/posts/869030609833316\', \]) /}
{param items} {call .item} {param name: \'Facebook\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/ZZPdzvlpK9r_Df9C3M7j1rNRi7hhHRvPhlklJ3lfi5jk86Jd1s0Y5wcQ1QgbVaAP5Q=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.facebook.katana\',
\'iOS\': \'https://itunes.apple.com/us/app/facebook/id284882215\', \] /}
{/call} {call .item} {param name: \'Messenger\' /} {param imgSrc:
\'https://lh5.ggpht.com/0VYAvZLR9YhosF-thqm8xl8EWsCfrEY_uk2og2f59K8IOx5TfPsXjFVwxaHVnUbuEjc=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.facebook.orca\',
\'iOS\': \'https://itunes.apple.com/us/app/messenger/id454638411\', \]
/} {/call} {call .item} {param name: \'Workplace\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/D77zPWACCJG-AfXpzSsVJmM9Om2-Vj4ltstKINR22GFQBAv7zYhdzKQANWjLkrhvVw=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.facebook.work\',
\'iOS\':
\'https://itunes.apple.com/us/app/workplace-by-facebook/id944921229\',
\] /} {/call} {call .item} {param name: \'Instagram\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/aYbdIM1abwyVSUZLDKoE0CDZGRhlkpsaPOg9tNnBktUQYsXflwknnOn2Ge1Yr7rImGk=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.instagram.android\',
\'iOS\': \'https://itunes.apple.com/us/app/instagram/id389801252\', \]
/} {/call} {call .item} {param name: \'Ads Manager\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/ODKlFYm7BaNiLMEEDO2b4DOCU-hmS1-Fg3_x\_lLUaJZ0ssFsxciSoX1dYERaWDJuEs8=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.facebook.adsmanager\',
\'iOS\':
\'https://itunes.apple.com/us/app/facebook-ads-manager/id964397083\', \]
/} {/call} {call .item} {param name: \'Pages Manager\' /} {param imgSrc:
\'https://lh4.ggpht.com/vcyZimfIRlWrLarEpIj7MMSuqgwIkF4bx5nArKhFWsEqGclnPTAeLLK4cFiQ5QscRIEc=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.facebook.pages.app\',
\'iOS\':
\'https://itunes.apple.com/us/app/facebook-pages-manager/id514643583\',
\] /} {/call} {/param} {/call} {call .company} {param name: \'Brainium
Studios\' /} {param items} {call .item} {param name: \'Sudoku\' /}
{param imgSrc:
\'https://lh6.ggpht.com/m92klrf80HKcoOW10p565ooRzYsP7ktAgDLGT6QnK2KrfMxgcxsfgqJ1LwE08J8z7_br=w100\'
/} {param links: quoteKeysIfJs(\[ \'iOS/Android\':
\'http://www.brainiumstudios.com/site/sudoku.html\', \]) /} {/call}
{call .item} {param name: \'Blackjack\' /} {param imgSrc:
\'https://lh4.ggpht.com/9n8paiE9nfV380CK45QjdgRZ4xCVOx_LH8Ic3t-ITwjVVlCtrUOaQOv19CLFBnHCbb8=w100\'
/} {param links: quoteKeysIfJs(\[ \'iOS/Android\':
\'http://www.brainiumstudios.com/site/blackjack.html\', \]) /} {/call}
{call .item} {param name: \'Freecell\' /} {param imgSrc:
\'https://lh3.ggpht.com/c0l_lmDA-LB0meyB6tVik1gdi_i0z42_RPYjhYHZAiJDSZetuCxWDcqJl3INzI_iyz0=w100\'
/} {param links: quoteKeysIfJs(\[ \'iOS/Android\':
\'http://www.brainiumstudios.com/site/freecell.html\', \]) /} {/call}
{call .item} {param name: \'Jumbline 2\' /} {param imgSrc:
\'https://lh3.ggpht.com/QZSc3YEppWF7VDjms6X1vCBs5mW3r03pcqPmtTj_86PX9fUDkTh9PXBqxIvdGVE1FJou=w100\'
/} {param links: quoteKeysIfJs(\[ \'iOS/Android\':
\'http://www.brainiumstudios.com/site/jumbline.html\', \]) /} {/call}
{call .item} {param name: \'Spider\' /} {param imgSrc:
\'https://lh5.ggpht.com/KfdGhIv4Cp9ysjb67avoNLWAgVjjbBGjTtEw1EM6L_s00Oj_UeXJun-tj2ynxWwCZA=w100\'
/} {param links: quoteKeysIfJs(\[ \'iOS/Android\':
\'http://www.brainiumstudios.com/site/spider.html\', \]) /} {/call}
{/param} {/call} {call .company} {param name: \'Uber\' /} {param
moreInfo: quoteKeysIfJs(\[ \'Uber Engineering\\\'s iOS Monorepo\':
\'https://eng.uber.com/ios-monorepo/\', \]) /} {param items} {call
.item} {param name: \'Uber\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/iyt_f1j2d2ildbFLDlS0Qf36NJMeRVZFBetcg-pmrkdQtN9C1wUTaFhloKUcwVVfQeg=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.ubercab\', \'iOS\':
\'https://itunes.apple.com/us/app/uber/id368677368\', \] /} {/call}
{call .item} {param name: \'Uber Partner\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/71RQti5COPiUU6syMYePBeCozfE6xRwm-1ONbqe6TpsOP1nBj4Z4Y4QPpaO_F-o2v5s=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.ubercab.driver\',
\'iOS\': \'https://itunes.apple.com/us/app/uber-driver/id1131342792\',
\] /} {/call} {call .item} {param name: \'UberEATS\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/-M679h76FAjLJI6sv9VYUGKLXK7jdG1_95XRV8DJslC1e3_2QAesO7H7jDtDYEObTc3w=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.ubercab.eats\',
\'iOS\':
\'https://itunes.apple.com/us/app/ubereats-uber-for-food-delivery/id1058959277\',
\] /} {/call} {call .item} {param name: \'Uber Freight\' /} {param
imgSrc:
\'https://lh3.googleusercontent.com/\_fsFvGVNIw6R3Llaj7ATtTOtRr3OiUIwHXtVcetCfPA8VGl4y0fMV59PFIbEfmzoDQ=w100\'
/} {param links: \[ \'Android\':
\'https://play.google.com/store/apps/details?id=com.ubercab.freight\',
\'iOS\': \'https://itunes.apple.com/us/app/uber-freight/id1183931851\',
\] /} {/call} {/param} {/call} {call .company} {param name: \'Others\'
/} {param items} {call .item} {param name: \'Airbnb\' /} {param imgSrc:
\'https://lh3.googleusercontent.com/BQnvuZR500pg2ulvv3FBmRI93ODz3AjNfbz92hCieuJLvmbGY36AKhETMTTfTDgpPQI=w100\'
/} {/call} {call .item} {param name: \'Lyft\' /} {param imgSrc:
\'https://lh5.ggpht.com/CfRup8ZMEbNpd4sf8PDUWzbnFIq0QINZpJ96M6V0-8wLmyqKD0ORSqPOq5EKdL1OskE=w100\'
/} {/call} {call .item} {param name: \'Easynvest\' /} {param imgSrc:
\'https://theme.zdassets.com/theme_assets/1130385/0290357291ec4f3e2975f9b58183a608414fbf8d.png\'
/} {/call} {/param} {/call}\

Want to be included in this page? Add yourself by{sp} [submitting a pull
request](https://github.com/facebook/buck/edit/master/docs/about/showcase.soy){target="_blank"}.

{/param} // content {/call} // buck.page {/template}

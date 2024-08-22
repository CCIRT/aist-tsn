![overwiew_cbs-switch drawio](https://github.com/user-attachments/assets/c21761e5-2815-445a-99a1-44aa605878cf)# AIST-TSN
AIST-TSN is an open source project developed by the National Institute of Advanced Industrial Science and Technology (AIST), Japan.
It introduces the hardware design of an L2 network switch design supporting Time Sensitive Networks (TSN). 
We aim to provide an open platform that can be used as a reference design so scientists can implement their desired functionalities and make the different evaluations and comparisons to highlight the appropriate design choices for a given TSN system.

This repository includes two flavors of an L2 TSN switch supporting two different scheduling algorithms. Both designes are implemented and validated on an AMD Xilinx KC705 FPGA evaluation board:

- L2 switch supporting CBS:
  - [Specification]()
  - [FPGA design docs]()
![Uploading ov<svg host="65bd71144e" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" width="841px" height="341px" viewBox="-0.5 -0.5 841 341" content="&lt;mxfile&gt;&lt;diagram id=&quot;ebE0OGtsRTfp5YOnq2ey&quot; name=&quot;ページ1&quot;&gt;7V1tc5s4EP41mUk/JIN452PiNG3vLtfMZeau/UgNtZkSk8Mkce7Xn2wjG7SyEXTFm5svMTLI8Oxqd/VoV5wZk8fVh9R/mt8lQRif6VqwOjNuznSdOKZJ/61b3rYtJmuYpVGQn7RveIj+C/NGLW99joJwWToxS5I4i57KjdNksQinWanNT9PktXza9yQu/+qTPwtBw8PUj2HrP1GQzbetru7s2z+G0WzOfpnY3vabR5+dnD/Jcu4HyWuhyXh/ZkzSJMm2nx5XkzBeg8dw2V53e+Db3Y2l4SKTuoAY20te/Pg5f7r8zrI39rjhIrhao0aPFsmCNl7Ps8eYHhH6MU2eF0G47k6jR4G/nG8O1l/Bm8nvLwxK+Oa39iFMHsMsfaMnvO5RtXKk5gVAWVsaxn4WvZSl4ufCne262/3CfRLRO9G1Fesm7ydXQ8PWyl0sk+d0GuZXFVHkOjI979Ih2v7PLPVLNK7fzE9nYQb6pR8KKOybNjI7JD/zdOXnuEjyc5yy/Iz2xEeqxVeW0Os8ysKHJ3+6/vaV2teyOL9HcTxJ4iTdC/ugGF/CNAtXRwWZf2twI4UBXZSzKxC0oWuHhVrC7RhImoSO9wEkswzSTm+KKOkClHReb5ugZA0CI6JXKhKxVSkSVKP7j1/PdDumP3L9LaWfZutPrvueWCzUaAofBlacedthVwBLhJWJAJVuQy9Cjf5Dfpik2TyZJQs/fr9vLT4+fer07UsO1ebg6/rg0mKHN6vilzdv7GgVZV9YH/Tz9irdyg/3V60P2EVlwRxEfusNcou/bdpa8vyRLUnnVs9rUc/rvxVOeFq7jeVhp2byVsTgIriq802NE/T2Dpq6KAcMmrurCZ5pCcLv/vNmAGJYYLt6xJiKRowLcPp94mhW51aEd92mwCmJfBICJB6A5PO9ZpAL8rfbOSy8IxLAIgpocOIZgMsfV39CP/TXb2b36sPj1OaQQg+O148d0Wn8VRzNFrQtS55wUNJ5wyMI/USuGiXyIwIrU+2sy8BJuG5die+W8tZEh+6aUSp47loab904ijecYzNktBIyznFkdnIgZTk4VXJoDCnjgrqAFIz0YYXmbnuhORFYQTn1qzUwG5sBOfUzBOqnd6Z+kAQdkEcW6J4yj6w5qK6mh4ppQsV0ZWlPBXbxuGsfhqsRQErQJ9vSkA6cBRLNVNS5GnMErsYSqJ/ZmfpBnnY4rkake+pcjTd2V2NDxfQ6DMGPu/ZhuBoBpMTpDFJ72K7GkGQxcFzN8RWHYbgawbICU4IO1A9S98NxNSLdU+ZqIFENdXGfQzGN/eUymvZfGzWojbJxTzsJHIZzQOi1E3D4QMXiOsJL2WC/hKEsPfKcojma1itlIZyyEH7oyyqLx/XjqdMViQWMARoWga7IxlgDUxXC6wrfEaKu1EvEHIpdEURE/fJBQMRNkwiB0vEdIeoKJBFuP91+BvrSj6wMUyKPSVVoZ0KkHl6jbDqHYTBtpq3a7c11T3G0JLJbhDkLGEkLVm0msGEGmJwHcqFZsTqjTkyY+zO5fuipFtkdjkYL+rhJnEx/wME4SRYvlz1F0Okwy8yqTdKhe/cmYd9P+mh+ekf46Z106M+LzhQXbuC7bAvaCCjJivDuoEh6EkpZvJgMiq7m7f/cZlIDjq+iXzypsR8uMrhJur41yNZS65GV5bXM0uRHyCXRC/Lq/TwdbUrlGtJ2kKf2GAXBZnlDZPIks59rxGvNwgwM82bDCXOONzkdvAX5HMrw1g/hDa3TWPGWTf1FwRsGQDneMKVwrHiLmH1leEtURQ3d69qgYIR6R7sQ01jNvC6YKFT0i+h14cLVuf+upwNErmK2xmjhgyiBeRIWEWIMF1iXMaqqL5YzXprCyK5ytFz25ZXKuCrPZxEpVtkX0ZpUAFam3/SImRYpQ3cpyOxuhlln12IKMhuvA+W+20QKzpk6pGwdXWB7O6Ns2d0Mk7JtU4kkKNsCYva/z8mmOUmDML2YbuG42nSQnl9cFNvfbdBhVwyS+W1TELUrAZQyv/jld3LULw1MLgtzEI3rsCkRrGttEcEOTAqFgh34lBQQwdz+SKThlBQQwRX9IkoNTklHJzVAJKzRtQose0P6Hrivin4RpQaD6vNvp0ok6ALeTRWRwCQ+ViLBFXhEF33uiEIkMOsgTSTY2ERCE1JpSESCSBm6KzBjdzNIIqHNAjM2XodJJLSKVO39LlQSCa6oQruzcmJ2N4MkElpVIrgU94tI6EQQ/Uohw99cQZJIcNQQCXZbRIJ7ghlluqWGSKjqF1FqCLWGfZcaTyRs0LWbSQq4LEFfeNLxYPB8Pj1ZwkCwOa8qwsATjIIxEQaeYL8rD32OiEIYGKQeYcC2ZkYjDAQ7IYyLMBApQ3fbBHhwhW84hEGb2wR4cKo3IMKgVaQar1WqIAw80T47nW0K48H1v+EQBq0qEVxy+0UYdCKI4xtxtU0Y4G+RJUcYGAZS0Zmht0UR7LahHvNsk+cIDHIc3qYcQVW/mGJD2Dek72LjSYINvEgkgagvTPHAiPk8OFWWYPdmnhZYAiLYPfPYwBj12852+43UHS0un0XFd4T5frN62W6jFpiu45RD8/LT+cAEU3718t7GLT9+o7DGAlO34xgh9VaFRiUw8AK+phaSfzGoUgtZb0Fo1ALTK2ZGTeVX1S+iOGtuDzlucTY1mEB+Cg2mDudanxbLKAhp2+39hysgvdZf4MahKrk9BEq8LXiF2+3dT64NIEDCv25L8u07KJAYdZPhmo/anxyOLj+Kmu5s6B5aGFYwHA24yHI6K/AAaFHtvwEVG2UTbKPuok1/FLvpttEAb4Vv+jbgTPh0alF4oEWFk+oUu27CY28UG7z1uqlig44wFRvOOE+HDQVAi4qslCl23YW53ih24w25gSFRtyH3ruuT3IYIAC2i+VUptqkD5FewiqwfwCNgDQpvJasBUOYzJlzMOiWsRVWx6rCGk5uTwlqQUKwOa7hUeEpYi5ZlkbCmh2myzpzaO1b6UPO7JAjXZ/wP&lt;/diagram&gt;&lt;/mxfile&gt;">
    <defs/>
    <g>
        <path d="M 460 320 L 459.71 60" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <path d="M 740 320 L 739.71 60" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <rect x="260" y="20" width="580" height="320" fill="none" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <rect x="300" y="60" width="520" height="260" fill="none" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <rect x="80" y="20" width="160" height="320" fill="none" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <rect x="140" y="80" width="60" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 58px; height: 1px; padding-top: 100px; margin-left: 141px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                PHY
                                <br/>
                                88E1510
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="170" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    PHY...
                </text>
            </switch>
        </g>
        <path d="M 360 90 L 400 90 L 400 100 L 433.63 100" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 438.88 100 L 431.88 103.5 L 433.63 100 L 431.88 96.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="320" y="80" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 100px; margin-left: 321px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                MAC
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="340" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    MAC
                </text>
            </switch>
        </g>
        <rect x="260" y="0" width="50" height="20" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 48px; height: 1px; padding-top: 10px; margin-left: 261px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                KC705
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="285" y="14" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    KC705
                </text>
            </switch>
        </g>
        <rect x="80" y="0" width="80" height="20" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 78px; height: 1px; padding-top: 10px; margin-left: 81px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                OP031-1V8
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="120" y="14" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    OP031-1V8
                </text>
            </switch>
        </g>
        <rect x="80" y="80" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 100px; margin-left: 81px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                LAN
                                <br/>
                                RJ45
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="100" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    LAN...
                </text>
            </switch>
        </g>
        <rect x="220" y="60" width="60" height="260" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <path d="M 200 150 L 313.63 150" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 318.88 150 L 311.88 153.5 L 313.63 150 L 311.88 146.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 140 170 L 126.37 170" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 121.12 170 L 128.12 166.5 L 126.37 170 L 128.12 173.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="140" y="140" width="60" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 58px; height: 1px; padding-top: 160px; margin-left: 141px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                PHY
                                <br/>
                                88E1510
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="170" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    PHY...
                </text>
            </switch>
        </g>
        <path d="M 120 150 L 133.63 150" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 138.88 150 L 131.88 153.5 L 133.63 150 L 131.88 146.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="80" y="140" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 160px; margin-left: 81px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                LAN
                                <br/>
                                RJ45
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="100" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    LAN...
                </text>
            </switch>
        </g>
        <path d="M 200 210 L 313.63 210" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 318.88 210 L 311.88 213.5 L 313.63 210 L 311.88 206.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 140 230 L 126.37 230" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 121.12 230 L 128.12 226.5 L 126.37 230 L 128.12 233.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="140" y="200" width="60" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 58px; height: 1px; padding-top: 220px; margin-left: 141px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                PHY
                                <br/>
                                88E1510
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="170" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    PHY...
                </text>
            </switch>
        </g>
        <path d="M 120 210 L 133.63 210" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 138.88 210 L 131.88 213.5 L 133.63 210 L 131.88 206.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="80" y="200" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 220px; margin-left: 81px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                LAN
                                <br/>
                                RJ45
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="100" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    LAN...
                </text>
            </switch>
        </g>
        <path d="M 200 270 L 313.63 270" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 318.88 270 L 311.88 273.5 L 313.63 270 L 311.88 266.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 140 290 L 126.37 290" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 121.12 290 L 128.12 286.5 L 126.37 290 L 128.12 293.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="140" y="260" width="60" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 58px; height: 1px; padding-top: 280px; margin-left: 141px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                PHY
                                <br/>
                                88E1510
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="170" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    PHY...
                </text>
            </switch>
        </g>
        <path d="M 120 270 L 133.63 270" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 138.88 270 L 131.88 273.5 L 133.63 270 L 131.88 266.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="80" y="260" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 280px; margin-left: 81px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                LAN
                                <br/>
                                RJ45
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="100" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    LAN...
                </text>
            </switch>
        </g>
        <path d="M 120 90 L 133.63 90" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 138.88 90 L 131.88 93.5 L 133.63 90 L 131.88 86.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 140 110 L 126.37 110" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 121.12 110 L 128.12 106.5 L 126.37 110 L 128.12 113.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 200 90 L 313.63 90" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 318.88 90 L 311.88 93.5 L 313.63 90 L 311.88 86.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 320 110 L 206.37 110" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 201.12 110 L 208.12 106.5 L 206.37 110 L 208.12 113.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="440" y="80" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 100px; margin-left: 441px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                FIFO
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="460" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    FIFO
                </text>
            </switch>
        </g>
        <rect x="520" y="80" width="80" height="220" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 78px; height: 1px; padding-top: 190px; margin-left: 521px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Switch
                                <br/>
                                with FDB
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="560" y="194" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Switch...
                </text>
            </switch>
        </g>
        <path d="M 680 100 L 713.63 100" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 718.88 100 L 711.88 103.5 L 713.63 100 L 711.88 96.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="640" y="80" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 100px; margin-left: 641px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                CBS
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="660" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    CBS
                </text>
            </switch>
        </g>
        <rect x="720" y="80" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 100px; margin-left: 721px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Clock
                                <br/>
                                Conv.
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="740" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Clock...
                </text>
            </switch>
        </g>
        <path d="M 380 110 L 366.37 110" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 361.12 110 L 368.12 106.5 L 366.37 110 L 368.12 113.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 480 99.71 L 513.63 99.71" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 518.88 99.71 L 511.88 103.21 L 513.63 99.71 L 511.88 96.21 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="0" y="80" width="80" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 78px; height: 1px; padding-top: 100px; margin-left: 1px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Port 0
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="40" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Port 0
                </text>
            </switch>
        </g>
        <rect x="0" y="140" width="80" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 78px; height: 1px; padding-top: 160px; margin-left: 1px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Port 1
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="40" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Port 1
                </text>
            </switch>
        </g>
        <rect x="0" y="200" width="80" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 78px; height: 1px; padding-top: 220px; margin-left: 1px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Port 2
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="40" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Port 2
                </text>
            </switch>
        </g>
        <rect x="0" y="260" width="80" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 78px; height: 1px; padding-top: 280px; margin-left: 1px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Port 3
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="40" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Port 3
                </text>
            </switch>
        </g>
        <path d="M 600 99.76 L 633.63 99.76" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 638.88 99.76 L 631.88 103.26 L 633.63 99.76 L 631.88 96.26 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="380" y="100" width="20" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 18px; height: 1px; padding-top: 110px; margin-left: 381px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (a)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="390" y="114" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (a)
                </text>
            </switch>
        </g>
        <path d="M 360 150 L 400 150 L 400 160 L 433.63 160" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 438.88 160 L 431.88 163.5 L 433.63 160 L 431.88 156.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 320 170 L 206.37 170" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 201.12 170 L 208.12 166.5 L 206.37 170 L 208.12 173.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="320" y="140" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 160px; margin-left: 321px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                MAC
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="340" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    MAC
                </text>
            </switch>
        </g>
        <rect x="440" y="140" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 160px; margin-left: 441px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                FIFO
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="460" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    FIFO
                </text>
            </switch>
        </g>
        <path d="M 680 160 L 713.63 160" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 718.88 160 L 711.88 163.5 L 713.63 160 L 711.88 156.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="640" y="140" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 160px; margin-left: 641px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                CBS
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="660" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    CBS
                </text>
            </switch>
        </g>
        <rect x="720" y="140" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 160px; margin-left: 721px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Clock
                                <br style="border-color: var(--border-color);"/>
                                Conv.
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="740" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Clock...
                </text>
            </switch>
        </g>
        <path d="M 380 170 L 366.37 170" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 361.12 170 L 368.12 166.5 L 366.37 170 L 368.12 173.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 480 159.71 L 513.63 159.71" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 518.88 159.71 L 511.88 163.21 L 513.63 159.71 L 511.88 156.21 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 600 159.76 L 633.63 159.76" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 638.88 159.76 L 631.88 163.26 L 633.63 159.76 L 631.88 156.26 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="380" y="160" width="20" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 18px; height: 1px; padding-top: 170px; margin-left: 381px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (b)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="390" y="174" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (b)
                </text>
            </switch>
        </g>
        <path d="M 360 210 L 400 210 L 400 220 L 433.63 220" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 438.88 220 L 431.88 223.5 L 433.63 220 L 431.88 216.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 320 230 L 206.37 230" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 201.12 230 L 208.12 226.5 L 206.37 230 L 208.12 233.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="320" y="200" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 220px; margin-left: 321px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                MAC
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="340" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    MAC
                </text>
            </switch>
        </g>
        <rect x="440" y="200" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 220px; margin-left: 441px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                FIFO
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="460" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    FIFO
                </text>
            </switch>
        </g>
        <path d="M 680 220 L 713.63 220" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 718.88 220 L 711.88 223.5 L 713.63 220 L 711.88 216.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="640" y="200" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 220px; margin-left: 641px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                CBS
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="660" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    CBS
                </text>
            </switch>
        </g>
        <rect x="720" y="200" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 220px; margin-left: 721px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Clock
                                <br style="border-color: var(--border-color);"/>
                                Conv.
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="740" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Clock...
                </text>
            </switch>
        </g>
        <path d="M 380 230 L 366.37 230" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 361.12 230 L 368.12 226.5 L 366.37 230 L 368.12 233.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 480 219.71 L 513.63 219.71" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 518.88 219.71 L 511.88 223.21 L 513.63 219.71 L 511.88 216.21 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 600 219.76 L 633.63 219.76" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 638.88 219.76 L 631.88 223.26 L 633.63 219.76 L 631.88 216.26 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="380" y="220" width="20" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 18px; height: 1px; padding-top: 230px; margin-left: 381px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (c)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="390" y="234" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (c)
                </text>
            </switch>
        </g>
        <path d="M 360 270 L 400 270 L 400 280 L 433.63 280" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 438.88 280 L 431.88 283.5 L 433.63 280 L 431.88 276.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 320 290 L 206.37 290" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 201.12 290 L 208.12 286.5 L 206.37 290 L 208.12 293.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="320" y="260" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 280px; margin-left: 321px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                MAC
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="340" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    MAC
                </text>
            </switch>
        </g>
        <rect x="440" y="260" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 280px; margin-left: 441px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                FIFO
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="460" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    FIFO
                </text>
            </switch>
        </g>
        <path d="M 680 280 L 713.63 280" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 718.88 280 L 711.88 283.5 L 713.63 280 L 711.88 276.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="640" y="260" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 280px; margin-left: 641px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                CBS
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="660" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    CBS
                </text>
            </switch>
        </g>
        <rect x="720" y="260" width="40" height="40" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 280px; margin-left: 721px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Clock
                                <br style="border-color: var(--border-color);"/>
                                Conv.
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="740" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Clock...
                </text>
            </switch>
        </g>
        <path d="M 380 290 L 366.37 290" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 361.12 290 L 368.12 286.5 L 366.37 290 L 368.12 293.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 480 279.71 L 513.63 279.71" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 518.88 279.71 L 511.88 283.21 L 513.63 279.71 L 511.88 276.21 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <path d="M 600 279.76 L 633.63 279.76" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 638.88 279.76 L 631.88 283.26 L 633.63 279.76 L 631.88 276.26 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="380" y="280" width="20" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 18px; height: 1px; padding-top: 290px; margin-left: 381px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (d)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="390" y="294" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (d)
                </text>
            </switch>
        </g>
        <path d="M 740 130 L 820 130" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <path d="M 740 189.71 L 820 190" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <path d="M 740 250 L 820 250" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <path d="M 300 130 L 460 130" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <path d="M 300 189.71 L 460 189.71" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <path d="M 300 250 L 460 250" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" stroke-dasharray="3 3" pointer-events="stroke"/>
        <rect x="300" y="40" width="80" height="20" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 78px; height: 1px; padding-top: 50px; margin-left: 301px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                Inside FPGA
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="340" y="54" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    Inside FPGA
                </text>
            </switch>
        </g>
        <rect x="220" y="40" width="60" height="20" fill="rgb(255, 255, 255)" stroke="rgb(0, 0, 0)" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 58px; height: 1px; padding-top: 50px; margin-left: 221px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                FMC
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="250" y="54" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    FMC
                </text>
            </switch>
        </g>
        <path d="M 760 220 L 773.63 220" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 778.88 220 L 771.88 223.5 L 773.63 220 L 771.88 216.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="780" y="200" width="23" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 21px; height: 1px; padding-top: 220px; margin-left: 781px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (c)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="792" y="224" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (c)
                </text>
            </switch>
        </g>
        <path d="M 760 160 L 773.63 160" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 778.88 160 L 771.88 163.5 L 773.63 160 L 771.88 156.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="780" y="140" width="23" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 21px; height: 1px; padding-top: 160px; margin-left: 781px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (b)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="792" y="164" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (b)
                </text>
            </switch>
        </g>
        <path d="M 760 280 L 773.63 280" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 778.88 280 L 771.88 283.5 L 773.63 280 L 771.88 276.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="780" y="260" width="23" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 21px; height: 1px; padding-top: 280px; margin-left: 781px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (d)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="792" y="284" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (d)
                </text>
            </switch>
        </g>
        <path d="M 760 100 L 773.63 100" fill="none" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="stroke"/>
        <path d="M 778.88 100 L 771.88 103.5 L 773.63 100 L 771.88 96.5 Z" fill="rgb(0, 0, 0)" stroke="rgb(0, 0, 0)" stroke-miterlimit="10" pointer-events="all"/>
        <rect x="780" y="80" width="23" height="40" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 21px; height: 1px; padding-top: 100px; margin-left: 781px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                (a)
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="792" y="104" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    (a)
                </text>
            </switch>
        </g>
        <rect x="600" y="100" width="40" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 110px; margin-left: 601px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                x8
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="620" y="114" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    x8
                </text>
            </switch>
        </g>
        <rect x="600" y="160" width="40" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 170px; margin-left: 601px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                x8
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="620" y="174" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    x8
                </text>
            </switch>
        </g>
        <rect x="600" y="220" width="40" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 230px; margin-left: 601px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                x8
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="620" y="234" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    x8
                </text>
            </switch>
        </g>
        <rect x="600" y="280" width="40" height="20" fill="none" stroke="none" pointer-events="all"/>
        <g transform="translate(-0.5 -0.5)">
            <switch>
                <foreignObject pointer-events="none" width="100%" height="100%" requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility" style="overflow: visible; text-align: left;">
                    <div xmlns="http://www.w3.org/1999/xhtml" style="display: flex; align-items: unsafe center; justify-content: unsafe center; width: 38px; height: 1px; padding-top: 290px; margin-left: 601px;">
                        <div data-drawio-colors="color: rgb(0, 0, 0); " style="box-sizing: border-box; font-size: 0px; text-align: center;">
                            <div style="display: inline-block; font-size: 12px; font-family: Helvetica; color: rgb(0, 0, 0); line-height: 1.2; pointer-events: all; white-space: normal; overflow-wrap: normal;">
                                x8
                            </div>
                        </div>
                    </div>
                </foreignObject>
                <text x="620" y="294" fill="rgb(0, 0, 0)" font-family="Helvetica" font-size="12px" text-anchor="middle">
                    x8
                </text>
            </switch>
        </g>
    </g>
    <switch>
        <g requiredFeatures="http://www.w3.org/TR/SVG11/feature#Extensibility"/>
        <a transform="translate(0,-5)" xlink:href="https://www.diagrams.net/doc/faq/svg-export-text-problems" target="_blank">
            <text text-anchor="middle" font-size="10px" x="50%" y="100%">
                Text is not SVG - cannot display
            </text>
        </a>
    </switch>
</svg>
erwiew_cbs-switch.drawio.svg…]()


- L2 switch supporting ATS:
  - [Specification]()
  - [FPGA design docs]()

## Licensing
Copyright (c) 2024 National Institute of Advanced Industrial Science and Technology (AIST)
All rights reserved.
This software is released under the MIT License.

When using the provided designs in this repository, please refer to the following citations:
- CBS:
> _Akram BEN AHMED, Takahiro HIROFUCHI, and Takaaki FUKAI "FPGA-based Network Switch Architecture Supporting Credit Based Shaper for Time Sensitive Networks", The 29th IEEE International Conference on Emerging Technologies and Factory Automation (ETFA2024), Sep 2024_

- ATS:
> _Akram BEN AHMED, Takahiro HIROFUCHI, and Takaaki FUKAI, "Hardware design and Evaluation of an FPGA-based Network Switch Supporting Asynchronous Traffic Shaping for Time Sensitive Networking", IEEE Access, Sep 2024_
 
## Build device
**NOTE:** ⚠️ A license is required to synthesize Vivado project for KC705.
The design was implemented and validated using the following environment:
- Ubuntu 20.04.3 LTS
- CMake 3.14 or later
- Vivado v2022.1
  -Set Vivado to ```PATH```
- Set ```XILINXD_LICENSE_FILE``` to environment variables


All designs will be built by running the command below.
```
cd <Repository top>
./build_device.sh impl_all
```

Bitstreams will be generated below.

-L2 switch with ATS
  -build-device/vivado/ats-switch/ats-switch.prj/ats-switch.runs/impl_1/design_1_wrapper.bit

-L2 switch with CBS
  -build-device/vivado/cbs-switch/cbs-switch.prj/cbs-switch.runs/impl_1/design_1_wrapper.bit

## Directories
├── 3rdparty   : 3rd-party projects  
├── cmake      : Common CMake files  
├── device     : Source code for device including FPGA  
├── docs       : Documentation  
├── evaluation : Evaluation experiments and results  
└── util       : Scripts for FPGA register modification  


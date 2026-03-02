================================================================================
                        UNIPIA 이메일 템플릿 가이드
================================================================================

[파일 구조]
--------------------------------------------------------------------------------
/unipia1/
├── unipia_mail.html      # 최종 이메일 템플릿 (메인 파일)
├── HTML_png1.5.png       # 배경 이미지 (버튼 없는 버전, 600x2005px)
├── google.png            # Google Play 버튼 이미지
├── Apple.png             # App Store 버튼 이미지
├── Hint.png              # 힌트 버튼 이미지
├── HTML_SVG.svg          # 원본 SVG 파일 (참고용)
├── HTML_SVG 4 1.svg      # 원본 SVG 파일 (참고용)
├── HTML_SVG 4 1.png      # 원본 PNG 파일 (참고용)
└── README.txt            # 이 파일


[이미지 URL 수정 방법]
--------------------------------------------------------------------------------
현재 모든 이미지는 GitHub Pages를 통해 호스팅되고 있습니다.

현재 URL 형식:
https://jsm1007.github.io/unipia1/[파일명]

예시:
- https://jsm1007.github.io/unipia1/HTML_png1.5.png
- https://jsm1007.github.io/unipia1/google.png
- https://jsm1007.github.io/unipia1/Apple.png
- https://jsm1007.github.io/unipia1/Hint.png


[다른 GitHub 계정으로 변경하는 방법]
--------------------------------------------------------------------------------
1. 본인의 GitHub 계정에 새 저장소를 만듭니다.
   예: https://github.com/[본인계정]/[저장소명]

2. 저장소 Settings > Pages에서 GitHub Pages를 활성화합니다.
   - Source: Deploy from a branch
   - Branch: main (또는 master)

3. 이미지 파일들을 저장소에 업로드합니다.

4. unipia_mail.html 파일에서 모든 이미지 URL을 수정합니다:

   변경 전: https://jsm1007.github.io/unipia1/
   변경 후: https://[본인계정].github.io/[저장소명]/

   수정해야 할 위치 (총 5곳):
   - 배경 이미지 (background 속성): HTML_png1.5.png
   - 상단 Google 버튼: google.png
   - 상단 Apple 버튼: Apple.png
   - 힌트 버튼: Hint.png
   - 하단 Google 버튼: google.png
   - 하단 Apple 버튼: Apple.png


[버튼 링크 수정 방법]
--------------------------------------------------------------------------------
unipia_mail.html 파일에서 href 속성을 찾아 수정합니다:

1. Google Play 링크:
   href="https://play.google.com/store/apps/details?id=com.unipia.unipia&hl=en_GB"

2. App Store 링크:
   href="https://apps.apple.com/kr/app/unipia-uk-student-community/id1608830229?l=en_GB"

3. 힌트 페이지 링크:
   href="https://unipia.uk/post/?id=1206"


[레이아웃 구조 설명]
--------------------------------------------------------------------------------
이 템플릿은 퍼센트 기반 반응형 레이아웃을 사용합니다.
Gmail 모바일 앱에서도 정상적으로 반응형이 작동합니다.

spacer 계산 방식 (padding-top 퍼센트):
- 상단 버튼까지: 62.17%
- 힌트 버튼까지: 214.33%
- 하단 버튼까지: 24.17%
- 하단 여백: 8.83%

버튼 위치 (padding으로 조절):
- 상단/하단 버튼: padding: 0 22%
- 힌트 버튼: padding: 0 35%


[이메일 발송 방법]
--------------------------------------------------------------------------------
1. unipia_mail.html 파일의 전체 내용을 복사합니다.
2. 이메일 클라이언트에서 HTML 모드로 붙여넣기 합니다.
   - Gmail: "HTML로 메일 보내기" 확장 프로그램 사용
   - 기타: 이메일 마케팅 서비스 (Mailchimp, SendGrid 등) 사용


[주의사항]
--------------------------------------------------------------------------------
- 이미지는 반드시 외부 URL로 호스팅되어야 합니다.
- 로컬 파일 경로는 이메일에서 작동하지 않습니다.
- GitHub Pages 활성화 후 반영까지 몇 분 소요될 수 있습니다.


================================================================================
                              문의: UNIPIA Team
================================================================================

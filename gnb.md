[프롬프트 제목: Apple Style Glassmorphism GNB - Tailwind CSS Version]

1. 핵심 컨셉 (Design Goal):
"Apple의 디자인 언어를 따르는 미니멀한 글래스모피즘 GNB를 제작해줘. Tailwind CSS를 사용하여 유지보수가 쉽고 세련된 UI를 만드는 것이 목표야. 신성민님의 포트폴리오(화이트 배경, 블루 포인트) 무드에 최적화해줘."

2. 레이아웃 및 테일윈드 설정 (Tailwind Styling):

구조: fixed top-0 w-full 설정을 기반으로 하며, 중앙 정렬된 max-w-5xl 컨테이너 안에 배치.

유리 질감: - bg-white/70 투명도와 backdrop-blur-md 유틸리티 사용.

border border-white/40와 rounded-2xl을 적용하여 디바이스 UI 느낌 강조.

스크롤 애니메이션: - JavaScript를 이용해 특정 스크롤 지점 이후 py-2, shadow-sm, mx-4 등의 클래스를 동적으로 추가/제거.

모든 수치 변화에는 transition-all duration-500을 적용하여 부드럽게 변하도록 함.

3. 인터랙션 및 포인트 (Interactions):

메인 컬러: Tailwind 기본 색상인 text-blue-600 또는 커스텀 컬러 #2D7FF9 사용.

Josh Style 호버 애니메이션:

메뉴 링크(<a>)에 group 클래스 부여.

하단 언더라인을 absolute bottom-0 left-0 w-0 h-0.5 bg-[#2D7FF9] transition-all duration-300 ease-[cubic-bezier(0.34,1.56,0.64,1)] group-hover:w-full로 구현.

로고 스타일: font-black, tracking-tighter, text-xl 클래스로 타이포그래피 임팩트 부여.

4. 기술적 요구사항:

Framework: HTML + Tailwind CSS (CDN 방식 또는 PostCSS 환경 모두 호환 가능하게).

Responsive: 모바일에서는 메뉴를 숨기거나 간격을 조절하는 hidden md:flex 패턴 적용.

Logic: 스크롤 위치에 따라 상단 바의 외형이 바뀌는 간단한 Vanilla JS 스크립트 포함.

5. 최종 결과물 요건:

Tailwind CSS 클래스만으로 모든 스타일이 완결된 단일 HTML 파일 형태로 제공할 것.

스크린샷의 '그리드 배경'과 잘 어울리는 투명도를 유지할 것.
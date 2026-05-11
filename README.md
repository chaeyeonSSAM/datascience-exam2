# 관리자 로그인 수정본

## 반영 내용
- 로그인 화면에서 테스트 아이디/비밀번호 노출 제거
- 로그인 입력칸 기본값 제거 유지
- autocomplete/autocapitalize/spellcheck 비활성화
- 관리자 아이디 `admin` 입력 시 `admin@gwangmun.edu`로 Supabase Auth 로그인
- 로그인 실패 시 Supabase Auth의 실제 오류 메시지를 화면에 표시하고 Console에도 출력

## 관리자 로그인이 계속 안 될 때
Supabase > Authentication > Users에서 `admin@gwangmun.edu`를 삭제 후 다시 Add user로 생성하세요.

- Email: admin@gwangmun.edu
- Password: gm11154
- Auto Confirm 또는 Confirm user 처리

그리고 GitHub Pages에 `index.html`을 다시 업로드한 뒤 Ctrl+F5 또는 주소 뒤에 `?v=adminfix1`을 붙여 접속하세요.

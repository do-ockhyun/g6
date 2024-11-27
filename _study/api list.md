
그누보드6
 0.1.0 
OAS 3.1


Authorize

## 인증


POST
/api/v1/token
Access/Refresh Token 발급


POST
/api/v1/token/refresh
Access Token 재 발급

## 게시판


GET
/api/v1/boards/{bo_table}/writes
게시판 조회



POST
/api/v1/boards/{bo_table}/writes
게시판 글 작성



GET
/api/v1/boards/{bo_table}/writes/{wr_id}
게시판 개별 글 조회



POST
/api/v1/boards/{bo_table}/writes/{wr_id}
게시판 개별 글 조회(비밀글)



PUT
/api/v1/boards/{bo_table}/writes/{wr_id}
게시판 글 수정



DELETE
/api/v1/boards/{bo_table}/writes/{wr_id}
게시판 글 삭제



POST
/api/v1/boards/{bo_table}/writes/delete
게시글 일괄 삭제



POST
/api/v1/boards/{bo_table}/writes/{wr_id}/delete
게시판 비회원 글 삭제



GET
/api/v1/boards/{bo_table}/{sw}
게시글 복사/이동 가능 목록 조회



POST
/api/v1/boards/{bo_table}/{sw}
게시글 복사/이동



POST
/api/v1/boards/{bo_table}/writes/{wr_id}/files
파일 업로드



GET
/api/v1/boards/{bo_table}/writes/{wr_id}/files/{bf_no}
파일 다운로드



POST
/api/v1/boards/{bo_table}/writes/{wr_id}/comments
댓글 작성



PUT
/api/v1/boards/{bo_table}/writes/{wr_id}/comments
댓글 수정



DELETE
/api/v1/boards/{bo_table}/writes/{wr_id}/comments/{comment_id}
댓글 삭제



POST
/api/v1/boards/{bo_table}/writes/{wr_id}/comments/{comment_id}/delete
게시판 비회원 댓글 삭제



GET
/api/v1/config/board
게시판 설정 조회

## 캡차


POST
/api/v1/captcha/recaptcha/verify
구글 reCAPTCHA 유효성 검사

## 환경설정


GET
/api/v1/config/html
HTML 설정 조회


GET
/api/v1/config/policy
회원가입 약관 조회


GET
/api/v1/config/member
회원가입 설정 조회


GET
/api/v1/config/memo
쪽지 발송 시, 설정 포인트 조회


GET
/api/v1/config/board
게시판 설정 조회

## 회원


GET
/api/v1/config/policy
회원가입 약관 조회


GET
/api/v1/config/member
회원가입 설정 조회


POST
/api/v1/members
회원 가입


PUT
/api/v1/members/{mb_id}/email-certification/change
인증 이메일 변경


PUT
/api/v1/members/{mb_id}/email-certification
회원가입 메일인증 처리


GET
/api/v1/members/me
현재 로그인 회원 정보 조회



POST
/api/v1/members/password_certification
비밀번호 확인



GET
/api/v1/members/{mb_id}
회원 정보 조회



PUT
/api/v1/member
회원 정보 수정



DELETE
/api/v1/member
회원 탈퇴



PUT
/api/v1/member/image
회원 아이콘&이미지 수정



POST
/api/v1/members/search/id
회원 아이디 찾기


POST
/api/v1/members/search/password
비밀번호 재설정 메일 발송


PATCH
/api/v1/members/{mb_id}/password/{token}
비밀번호 재설정

## 쪽지


GET
/api/v1/config/memo
쪽지 발송 시, 설정 포인트 조회


GET
/api/v1/member/memos
쪽지 목록 조회



POST
/api/v1/member/memos
쪽지 전송



GET
/api/v1/member/memos/{me_id}
쪽지 조회



DELETE
/api/v1/member/memos/{me_id}
쪽지 삭제



PATCH
/api/v1/member/memos/{me_id}/read
쪽지 읽음 처리


## 컨텐츠


GET
/api/v1/contents
컨텐츠 목록 조회


GET
/api/v1/contents/{co_id}
컨텐츠 조회

## 현재 접속자


GET
/api/v1/members/current-connect
현재 접속자 목록 조회


## FAQ


GET
/api/v1/faqs
FAQ 분류 목록 조회


GET
/api/v1/faqs/{fm_id}
FAQ 분류 > 내용 목록 조회

## 게시판그룹


GET
/api/v1/groups/{gr_id}/boards
게시판그룹 목록 조회


## 메뉴


GET
/api/v1/menus
메뉴 목록 조회

## 레이어 팝업


GET
/api/v1/newwins
레이어 팝업 목록 조회

## 포인트


GET
/api/v1/member/points
회원 포인트 내역 목록 조회


## 설문조사


GET
/api/v1/polls/latest
최신 설문조사 1건 조회


GET
/api/v1/polls/{po_id}
설문조사 조회



PATCH
/api/v1/polls/{po_id}/{item}
설문조사 참여



POST
/api/v1/polls/{po_id}/etc
기타 의견 등록



DELETE
/api/v1/polls/{po_id}/etc/{pc_id}
기타 의견 삭제


## 인기 검색어


GET
/api/v1/populars
인기 검색어 목록 조회


POST
/api/v1/populars
인기 검색어 등록

## Q&A


GET
/api/v1/qa/config
Q&A 설정 조회


GET
/api/v1/qas
Q&A 목록 조회



POST
/api/v1/qas
Q&A 등록



GET
/api/v1/qas/{qa_id}
Q&A 상세 조회



PUT
/api/v1/qas/{qa_id}
Q&A 수정



DELETE
/api/v1/qas/{qa_id}
Q&A 삭제



PUT
/api/v1/qas/{qa_id}/files
Q&A 파일 업로드



GET
/api/v1/qas/{qa_id}/files/{file_index}
Q&A 파일 다운로드


## 스크랩


GET
/api/v1/member/scraps
회원 스크랩 목록 조회



GET
/api/v1/member/scraps/{bo_table}/{wr_id}
회원 스크랩 등록 페이지 설정 조회



POST
/api/v1/member/scraps/{bo_table}/{wr_id}
회원 스크랩 등록



DELETE
/api/v1/member/scraps/{ms_id}
회원 스크랩 삭제


## 검색


GET
/api/v1/search
게시판 검색


## 최신글


GET
/api/v1/board-new
최신 게시글 목록


GET
/api/v1/board-new/writes
최신글 조회


GET
/api/v1/board-new/writes/{bo_table}
최신글 게시판별 조회


POST
/api/v1/board-new/delete
최신 게시글을 삭제


## 좋아요/싫어요


POST
/api/v1/boards/{bo_table}/writes/{wr_id}/{good_type}
좋아요/싫어요


## 자동저장


GET
/api/v1/autosaves
자동저장 목록



POST
/api/v1/autosaves
자동저장



GET
/api/v1/autosaves/count
자동저장글 개수



GET
/api/v1/autosaves/{as_id}
자동저장글 불러오기



DELETE
/api/v1/autosaves/{as_id}
자동저장글 삭제


## 방문자


GET
/api/v1/visit
방문자 집계 조회


POST
/api/v1/visit
방문자 접속 이력 생성

# 발견 문제점

## 1. WriteDAOImpl()생성 불가

```
mapper 파일에 'insert'의  parmeterType= 'url'오류
 parmeterType='com.lec.spring.WriteDTO' 
                ▼
 parmeterType='com.lec.spring.domain.WriteDTO' 로 변경
```

## 2. 수정 성공 오류
updateOk.jsp 파일오류
```
location.href = "view.do?uid=${uid}"
        ▼
location.href = "view.do?uid=${param.uid}";
```

## 3. 삭제 오류

```
변수명 오류
DELETE FROM test_write WHERE uid = #{uid}
                ▼
DELETE FROM test_write WHERE wr_uid = #{uid}               
```
 




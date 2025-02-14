# interparkProj


== 약관 목록 불러오기 요구 정의서
	GET  /api/termsApi/termList
	Request : null
	Response : {
		"termsList"[
			{	
				"termsId" : "1" ,					// 약관ID
				"termsTitle" : "개인정보 수집동의", 	// 약관제목
				"termsUrl" : "", 					// 약관 세부정보 팝업 Url
				"termsAttribute" : "", 				// 약관속성(필수,선택 등)
			}
		]
	} 
	
	Error :{
		error : "약관 페이지 불러오기에 실패하였습니다."
	}
	
== 약관 세부내역 불러오기 API 요구 정의서
API Url : /users/termsDetail

Request : 
	HTTP: Get
	/api/termsApi/{termsId}


Response : 
	"termsContents"[
		{
			"termsId" : integer ,		// 약관 ID
			"termsTitle : String,		// 약관 제목
			"termsContents" : String,	// 약관 내용
		}
	]	

Error : 
{
	error : "약관 페이지 정보를 불러오기에 실패하였습니다."
}



== 가입내역작성 API 요구 정의서
API Url : /users/singup
Request : 
Response : 
	"singupList"[
		{
			"termsId" : integer ,		// 약관 ID
			"termsTitle : String,		// 약관 제목
			"termsContents" : String,	// 약관 내용
		}
	]	

Error : 
{
	error : "회원가입 페이지 정보를 불러오기에 실패하였습니다."
}

 

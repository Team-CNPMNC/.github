# JobFit AI – Nền tảng Tuyển dụng & Đánh giá Độ tương thích Hồ sơ Ứng viên

Dự án phát triển nền tảng kết nối việc làm và sàng lọc hồ sơ tự động ứng dụng trí tuệ nhân tạo, xây dựng theo quy trình Scrum nhằm đáp ứng các tiêu chuẩn nghiệp vụ và kỹ thuật[cite: 1].

---

## 1. Product Vision

### Tầm nhìn sản phẩm
JobFit AI được thiết kế nhằm tối ưu hóa quy trình sàng lọc hồ sơ tuyển dụng ban đầu, giúp doanh nghiệp rút ngắn đáng kể thời gian đọc duyệt hồ sơ và nâng cao độ chính xác khi lựa chọn ứng viên tiềm năng thông qua khả năng trích xuất thông tin, so khớp ngữ nghĩa và tự động tóm tắt đánh giá bằng AI[cite: 1].

### Đối tượng nhận giá trị
* **Nhà tuyển dụng (HR / Recruiter):** Tiết kiệm thời gian đọc CV thủ công; nhận ngay điểm số tương thích (Match Score), bản tóm tắt phân tích điểm mạnh, khoảng trống kỹ năng (Skills Gap) và bộ câu hỏi phỏng vấn gợi ý[cite: 1].
* **Người tìm việc (Job Seeker):** Tiếp cận thông tin việc làm minh bạch, quy trình nộp hồ sơ trực quan và theo dõi trạng thái ứng tuyển theo thời gian thực[cite: 1].

---

## 2. Phân loại luồng AI (AI Flow)

Hệ thống kết hợp chặt chẽ hai cơ chế xử lý trí tuệ nhân tạo[cite: 1]:
* **AI-managed Flow (Tự động hóa hoàn toàn):**
  * Tự động bóc tách nội dung tập tin CV (`.pdf`, `.docx`) thành dữ liệu có cấu trúc[cite: 1].
  * Tự động so sánh ngữ nghĩa giữa CV và bản mô tả công việc (JD), tính toán điểm phù hợp tổng thể trên thang điểm 100[cite: 1].
* **AI-assisted Flow (Hỗ trợ con người ra quyết định):**
  * AI đóng vai trò trợ lý: sinh bản tóm tắt đánh giá sơ bộ và gợi ý câu hỏi phỏng vấn trọng tâm[cite: 1].
  * Nhà tuyển dụng là người nắm quyền quyết định cuối cùng trong việc chuyển trạng thái hồ sơ (Mời phỏng vấn, Từ chối, Đưa vào danh sách chờ)[cite: 1].

---

## 3. Danh sách tính năng chính (Features)

### 3.1. Phân hệ AI Cốt lõi (AI Features)
* **CV Parser (AI-managed):** Tự động đọc và chuẩn hóa dữ liệu từ CV (Thông tin liên hệ, Học vấn, Kỹ năng, Kinh nghiệm làm việc)[cite: 1].
* **Semantic Matcher & Scorer:** Phân tích độ tương thích ngữ nghĩa giữa năng lực ứng viên và yêu cầu công việc[cite: 1].
* **Fit Summary Generator (AI-assisted):** Sinh đoạn văn tóm tắt ngắn (3–4 câu) chỉ rõ điểm mạnh và kỹ năng còn thiếu so với JD[cite: 1].
* **Interview Questions Recommender:** Đề xuất 3–5 câu hỏi phỏng vấn xoay quanh kinh nghiệm thực tế của ứng viên[cite: 1].

### 3.2. Phân hệ Doanh nghiệp (HR Portal)
* **Quản lý tin tuyển dụng:** Tạo mới, chỉnh sửa nội dung và đóng tin tuyển dụng kèm JD chi tiết[cite: 1].
* **Bảng điều khiển quản lý ứng viên (Applicant Tracking Dashboard):** 
  * Hiển thị danh sách ứng viên theo từng bài đăng, tự động sắp xếp theo điểm Match Score từ cao xuống thấp[cite: 1].
  * Xem nhanh tóm tắt của AI, danh sách kỹ năng khớp / chưa khớp và câu hỏi gợi ý[cite: 1].
* **Ra quyết định hồ sơ:** Cập nhật trạng thái ứng viên (Đang xét duyệt, Mời phỏng vấn, Từ chối)[cite: 1].

### 3.3. Phân hệ Ứng viên (Candidate Portal)
* **Khám phá việc làm:** Tìm kiếm tin tuyển dụng theo từ khóa, địa điểm và hình thức làm việc[cite: 1].
* **Nộp hồ sơ trực tuyến:** Tải lên tập tin CV (`.pdf`, `.docx` dung lượng tối đa 5MB) để ứng tuyển[cite: 1].
* **Theo dõi tiến độ hồ sơ:** Xem danh sách việc làm đã nộp và trạng thái cập nhật theo thời gian thực[cite: 1].

---

## 4. Đặc tả yêu cầu phần mềm (Requirements)

### 4.1. Danh sách User Stories & Acceptance Criteria (AC)
* **US-01:** HR tạo bài đăng tuyển dụng mới kèm JD đầy đủ các trường thông tin và xác thực dữ liệu đầu vào[cite: 1].
* **US-02:** HR quản lý danh sách tin tuyển dụng, hỗ trợ chỉnh sửa nội dung và đóng nhận hồ sơ[cite: 1].
* **US-03:** Ứng viên tìm kiếm, lọc và xem thông tin chi tiết bài tuyển dụng[cite: 1].
* **US-04:** Ứng viên tải lên tập tin CV với giới hạn định dạng (`.pdf`, `.docx`) và dung lượng tối đa 5MB[cite: 1].
* **US-05:** Ứng viên theo dõi trạng thái xử lý hồ sơ đã nộp trên giao diện cá nhân[cite: 1].
* **US-06 (AI-managed):** Hệ thống tự động bóc tách dữ liệu CV thành định dạng JSON có cấu trúc[cite: 1].
* **US-07 (AI-managed):** Hệ thống chấm điểm tương thích ngữ nghĩa (Match Score 0–100) giữa CV và JD trong thời gian dưới 10 giây[cite: 1].
* **US-08 (AI-assisted):** Hệ thống sinh đoạn văn tóm tắt Fit Summary và gợi ý 3–5 câu hỏi phỏng vấn[cite: 1].
* **US-09:** Dashboard HR hiển thị danh sách ứng viên xếp theo điểm số kèm bộ lọc phân khúc[cite: 1].
* **US-10 (AI-assisted):** HR cập nhật trạng thái ứng viên và đồng bộ kết quả sang tài khoản ứng viên[cite: 1].

### 4.2. Yêu cầu phi chức năng (Non-Functional Requirements)
* **Hiệu năng:** Tác vụ phân tích CV và xử lý AI được đưa vào hàng đợi chạy ngầm (Background Task) để không chặn luồng phản hồi API.
* **Bảo mật:** Dữ liệu cá nhân của ứng viên chỉ hiển thị cho tài khoản nhà tuyển dụng có thẩm quyền.
* **Độ ổn định:** Đầu ra của mô hình ngôn ngữ lớn được kiểm soát nghiêm ngặt theo lược đồ JSON định sẵn (Structured Output).

---

## 5. Bộ công nghệ sử dụng (Tech Stack)

### Giao diện người dùng (Frontend)
* **Ngôn ngữ:** TypeScript
* **Thư viện nền tảng:** React (khởi tạo với Vite)
* **Điều hướng:** React Router DOM
* **Giao diện & Thành phần:** Tailwind CSS kết hợp Shadcn UI
* **Quản lý dữ liệu mạng:** TanStack Query (React Query)
* **HTTP Client:** Axios

### Máy chủ dịch vụ (Backend API)
* **Ngôn ngữ:** Python
* **Khung ứng dụng:** FastAPI
* **Máy chủ ứng dụng:** Uvicorn
* **Thư viện ORM:** SQLAlchemy
* **Kiểm tra lược đồ dữ liệu:** Pydantic
* **Xử lý tác vụ ngầm:** FastAPI Background Tasks
* **Xác thực:** Python-Jose (JWT) và Passlib (Bcrypt)

### Thành phần Trí tuệ nhân tạo (AI Engine)
* **Mô hình ngôn ngữ lớn:** Google Gemini API (gói chính thức `google-genai`, mô hình Gemini 1.5 Flash)[cite: 1]
* **Bóc tách tập tin PDF:** PyMuPDF (`fitz`)
* **Bóc tách tập tin Word:** python-docx

### Cơ sở dữ liệu và Lưu trữ (Database & Storage)
* **Hệ quản trị cơ sở dữ liệu:** SQLite (lưu trữ tập tin cục bộ `app.db`)
* **Lưu trữ tập tin CV:** Lưu trực tiếp trong thư mục `uploads/` trên máy chủ cục bộ

---

## 6. Kế hoạch triển khai Sprint (Scrum Implementation)

Dự án được triển khai qua 2 Micro-Sprints (mỗi ngày 1 Sprint)[cite: 1]:

| Sprint | Mục tiêu chính | Nhiệm vụ kỹ thuật hoàn thành | Cải tiến sau Sprint (Retrospective) |
| :--- | :--- | :--- | :--- |
| **Sprint 1** | Xây dựng khung Web MVP và bóc tách dữ liệu cơ bản[cite: 1] | US-01, US-02, US-03, US-04, US-06[cite: 1] | **Problem:** Xử lý file đồng bộ gây chậm API upload.<br>**Action Plan:** Đưa tác vụ AI vào FastAPI Background Tasks trong Sprint 2[cite: 1]. |
| **Sprint 2** | Hoàn thiện AI Engine, Dashboard HR và tích hợp toàn diện[cite: 1] | US-05, US-07, US-08, US-09, US-10[cite: 1] | **Problem:** Độ trễ gọi API AI đôi lúc mất 3–5 giây.<br>**Action Plan:** Bổ sung hiệu ứng Skeleton Loading trên UI khi chờ kết quả[cite: 1]. |

---

## 7. Hướng dẫn cài đặt và chạy thử (Installation & Setup)

### Yêu cầu môi trường
* Node.js phiên bản 18 trở lên
* Python phiên bản 3.10 trở lên

### Cài đặt Backend
```bash
# Di chuyển vào thư mục backend
cd backend

# Tạo và kích hoạt môi trường ảo
python -m venv venv
source venv/bin/activate  # Trên Windows dùng: venv\Scripts\activate

# Cài đặt các gói phụ thuộc
pip install -r requirements.txt

# Tạo tập tin cấu hình .env và bổ sung API Key
echo GEMINI_API_KEY="your_api_key_here" > .env

# Chạy máy chủ phát triển
uvicorn main:app --reload --port 8000

# DAT111-GROUP4
làm về tiền lương theo ngành nghề 


1 Giới thiệu dự án
1.1 Giới thiệu 
I.Giới thiệu về hiện trạng
- Trong bối cảnh thị trường lao động ngày càng cạnh tranh, việc phân tích dữ liệu nhân sự nội bộ và thị trường là vô cùng quan trọng. Báo cáo này giúp doanh nghiệp hiểu rõ hơn về xu hướng tuyển dụng, xây dựng chính sách đãi ngộ, và nắm bắt mức độ hài lòng của nhân viên, từ đó đưa ra các quyết định chiến lược về nhân sự.

- Dự án này được thực hiện dựa trên bộ dữ liệu lớn, bao gồm 85.665 dòng và 11 trường thông tin (Nhân Viên Chính Thức, experience, skills, job_fields, salary, salary_min, salary_max, unit, min_salary, max_salary, avg_salary, city, feedback).

II.Các bước xây dựng dữ liệu
Bước 1: Xác định Mục tiêu và Đối tượng
Xác định: Câu chuyện của bạn là gì? (Ví dụ: "Phân tích thị trường lương cho vị trí Quản lý tại TP.HCM", "Nhu cầu kỹ năng cho ngành IT", "So sánh lương giữa Hà Nội và TP.HCM").
Đối tượng: Ai sẽ xem câu chuyện này?
Người tìm việc: Họ quan tâm đến mức lương, kinh nghiệm, và kỹ năng cần thiết cho một vị trí cụ thể.
Công ty/HR: Họ quan tâm đến mức lương cạnh tranh, và những kỹ năng phổ biến cần có.
Bước 2: Thu thập và Phân tích Dữ liệu
Đây là bước quan trọng nhất cần xử lý dữ liệu thô:
Làm sạch & Chuẩn hóa:
Lương (salary, salary_min, salary_max, unit): Đây là cột cần xử lý phức tạp nhất. Chuẩn hóa đơn vị tiền tệ (VND, USD) về một đơn vị chung (ví dụ: VND) bằng cách sử dụng tỷ giá hối đoái hiện tại. Tính toán mức lương trung bình hoặc khoảng lương thống nhất.
Kinh nghiệm (experience): Chuyển đổi các chuỗi văn bản ("trên 1 năm", "5-7 năm") thành giá trị số hoặc phân loại thành các nhóm (Junior, Mid-level, Senior) để dễ phân tích.
Kỹ năng (skills) & Lĩnh vực (job_fields): Vì đây là dữ liệu văn bản (text), bạn cần trích xuất và đếm tần suất (Frequency Analysis) của các từ khóa kỹ năng/lĩnh vực phổ biến để biết thị trường đang cần gì.
Tìm kiếm Insight (Phân tích):
Mối liên hệ Lương - Kinh nghiệm: Mức lương thay đổi như thế nào theo cấp bậc (position_level) và kinh nghiệm (experience)?
Phân bổ theo Địa lý: Mức lương, nhu cầu tuyển dụng, và các vị trí phổ biến khác nhau như thế nào giữa các thành phố (city)?
Cầu Kỹ năng: Những kỹ năng nào (skills) đang được yêu cầu nhiều nhất cho các nhóm ngành (Ngành nghề/Nhóm ngành) có mức lương cao nhất?
Bước 3: Xây dựng Cấu trúc Câu chuyện
Chọn 1-3 insight quan trọng nhất để tạo thành cốt truyện:
Mở đầu (Vấn đề): "Thị trường việc làm năm nay có gì khác biệt về lương và yêu cầu kỹ năng?"
Thân bài (Phân tích):
Insight 1: Trình bày mức lương trung bình theo cấp bậc và kinh nghiệm. (VD: "Mức lương quản lý cao hơn 50% so với nhân viên, nhưng yêu cầu kinh nghiệm tối thiểu 5 năm").
Insight 2: Chi tiết về nhu cầu kỹ năng lớn nhất trong các ngành hot. (VD: "Ngành Kỹ thuật đòi hỏi kỹ năng X và Y nhiều nhất, với mức lương cao nhất").
Kết luận (Hành động): "Để có được mức lương A, ứng viên cần tập trung phát triển kinh nghiệm B và kỹ năng C."
Bước 4: Trực quan hóa Dữ liệu
Sử dụng các biểu đồ phù hợp để kể câu chuyện

Mối liên hệ
Mục tiêu
Loại Biểu đồ Khuyên dùng
Lương theo Kinh nghiệm/Cấp bậc
Cho thấy mối quan hệ, xu hướng
Biểu đồ Hộp & Râu (Box Plot) hoặc Biểu đồ Cột (Thanh).
Phân bổ vị trí theo Thành phố
So sánh nhu cầu giữa các khu vực
Biểu đồ Cột hoặc Bản đồ nhiệt (Heatmap).
Tần suất Kỹ năng yêu cầu
Cho thấy các kỹ năng phổ biến
Biểu đồ Cột (Bar Chart) hoặc Word Cloud (cho ấn tượng trực quan).




Bước 5: Truyền tải Câu chuyện
Tập trung vào các phát hiện đã được chuẩn hóa (mức lương đã quy đổi, kinh nghiệm đã phân nhóm).
Sử dụng tiêu đề hấp dẫn (VD: "Khoảng cách lương 20% giữa TP.HCM và Hà Nội") để làm nổi bật insight chính trên mỗi slide/trang.


1.2 Yêu cầu của công ty
Nêu yêu cầu 
Báo cáo này tập trung giải quyết các yêu cầu chính từ phía công ty, cụ thể là:
Phân tích và so sánh mức lương (trung bình, tối thiểu, tối đa) theo từng địa phương (thành phố).
Mục đích: Xác định các khu vực có chính sách đãi ngộ tốt và khu vực cần cải thiện, làm cơ sở để điều chỉnh khung lương cho cạnh tranh.
Đánh giá mức độ ảnh hưởng của kỹ năng (skills) đến mức lương.
Mục đích: Đánh giá mối quan hệ giữa các kỹ năng chuyên môn và mức lương thực nhận, từ đó xác định các nhóm kỹ năng nào đang có giá trị cao trên thị trường.
Phân tích mức độ hài lòng của nhân viên theo từng ngành và thành phố.
Mục đích: Phân tích cảm nhận (feedback) của nhân viên về mức lương theo lĩnh vực công việc và địa phương, nhằm hỗ trợ cải thiện chính sách nhân sự và môi trường làm việc.



Đánh giá tính khả thi (năng lực, khả năng của mình có thể thực hiện dự án này)
Các kỹ năng của nhóm:
Xử lý & Phân tích Dữ liệu:
Thành thạo sử dụng Excel trong việc làm sạch dữ liệu thô, thống kê cơ bản, và tổng hợp dữ liệu bằng PivotTable.
Có kiến thức nền về SQL, thực hiện được các thao tác như truy vấn, lọc, gộp, và tính toán dữ liệu trên tập dữ liệu lớn.
Trực quan hóa & Báo cáo (Power BI):
Biết cách nhập dữ liệu từ nhiều nguồn (CSV, Excel) và xử lý ban đầu bằng Power Query.
Từng thiết kế dashboard với biểu đồ cơ bản phục vụ mục tiêu trình bày số liệu và xu hướng.

Các kỹ năng của nhóm cần nâng cao:
Thành thạo Power BI nâng cao:
Power Query: Học cách xử lý dữ liệu phức tạp, tự động hóa quy trình làm sạch, chuẩn hóa định dạng, và xử lý dữ liệu lỗi.
DAX nâng cao: Viết được các công thức đo lường (Measures) và cột tính toán (Calculated Columns) nhanh, chuẩn và chính xác.
Thiết kế dashboard chuyên nghiệp: Phát triển dashboard động, có tính tương tác cao, và tuân thủ chuẩn báo cáo doanh nghiệp hiện đại.
Phân tích chuyên sâu:
Kết hợp công cụ phân tích: Dùng Excel Power Pivot hoặc Power BI Dataflows để mở rộng khả năng phân tích, mô hình hóa và trích xuất insight.
=> Với nền tảng kỹ năng sẵn có và định hướng nâng cao rõ ràng, nhóm em hoàn toàn có đủ năng lực để hoàn thành dự án này. 


2 Phân tích yêu cầu khách hàng
Tiến hành phân tích yêu cầu khách hàng theo các bước sau đây
2.1 Phân tích yêu cầu
Dựa vào bộ dữ liệu công cty cung cấp và các yêu cầu khách hàng gửi, tiến hành phân tích:
Dựa vào bộ dữ liệu công ty cung cấp (85.665 dòng) và 3 yêu cầu chính (phân tích lương theo địa điểm, ảnh hưởng của kỹ năng, và mức độ hài lòng), đây là phân tích chi tiết:
- Dữ liệu:
o   Bộ dữ liệu lớn (85.665 dòng) với 11 trường thông tin.
o   Dữ liệu bao gồm nhiều định dạng: số (salary, min_salary, max_salary), văn bản (job_title, skills, city, feedback), và phân loại (job_fields).
o   Cột skills và feedback là dữ liệu văn bản, cần được xử lý (trích xuất, phân loại) trước khi phân tích.
- Quản lý và lưu trữ: Dữ liệu được cung cấp dưới dạng file (ví dụ: CSV, Excel).
- Công nghệ: Yêu cầu các kỹ năng về làm sạch (Excel), thống kê (PivotTable), xử lý dữ liệu (Power Query) và trực quan hóa (Power BI).
Quyết định dùng công nghệ nào
Sử dụng kết hợp Excel (cho các tác vụ làm sạch, thống kê nhanh bằng PivotTable) và Power BI (cho việc xử lý dữ liệu phức tạp qua Power Query và xây dựng dashboard tương tác).
Giải thích vì sao chọn? Dựa vào yêu cầu nào của khách hàng?
Yêu cầu 1 & 3 (Lương theo thành phố & Mức độ hài lòng): Có thể được thực hiện hiệu quả bằng chức năng PivotTable 2 chiều của Excel, một kỹ năng mà nhóm đã thành thạo.
Yêu cầu 2 (Ảnh hưởng của kỹ năng): Đòi hỏi xử lý dữ liệu văn bản phức tạp từ cột skills. Power Query (trong cả Excel và Power BI) là công cụ lý tưởng để trích xuất, chuẩn hóa và phân loại các kỹ năng này.
Yêu cầu chung (Trực quan hóa): Power BI cho phép tạo dashboard tương tác, chuyên nghiệp, vượt trội hơn Excel trong việc trình bày dữ liệu và xu hướng (đáp ứng kỹ năng nhóm cần nâng cao).
Công nghệ (đã quyết định):
Dữ liệu: Dữ liệu thô từ CSV/Excel.
Quản lý và lưu trữ: Dữ liệu sẽ được nhập và xử lý trong mô hình dữ liệu của Power BI (hoặc Power Pivot của Excel).
Công nghệ: Excel (PivotTable) và Power BI (Power Query, DAX, Dashboards).
2.2 Câu chuyện dữ liệu
Ai đọc báo cáo này?
Báo cáo hướng đến hai nhóm chính:
Doanh nghiệp/HR: Muốn biết xu hướng lương, kỹ năng “hot” để xây chính sách lương thưởng hợp lý.


Người tìm việc: Muốn biết vị trí, kỹ năng, thành phố nào có lương cao để định hướng nghề nghiệp.
Vấn đề là gì? Ở mức độ nào?
Thị trường lao động cạnh tranh, lương và yêu cầu kỹ năng thay đổi nhanh.


Cả doanh nghiệp và ứng viên đều thiếu dữ liệu rõ ràng để ra quyết định.


Báo cáo giúp hiểu xu hướng lương, xác định kỹ năng ảnh hưởng, và đánh giá mức độ hài lòng của nhân viên theo thành phố, lĩnh vực.
Sử dụng phương pháp gì?
Làm sạch & chuẩn hóa dữ liệu: dùng Excel/Power Query để xử lý lương, kinh nghiệm, kỹ năng.


Phân tích dữ liệu: tính lương trung bình, tìm mối liên hệ giữa kinh nghiệm – lương, kỹ năng – lương.


Phân tích văn bản: tách và đếm kỹ năng phổ biến, đánh giá cảm xúc trong feedback.


Trực quan hóa: dùng Power BI hiển thị kết quả bằng biểu đồ cột, bản đồ, Word Cloud, biểu đồ tròn.


2.2.1 Đặt vấn đề
Mô tả thực trạng:
- Thị trường lao động đang cạnh tranh gay gắt, mức lương và yêu cầu kỹ năng thay đổi nhanh.
- Doanh nghiệp cần hiểu rõ xu hướng tuyển dụng, chính sách đãi ngộ, và mức độ hài lòng của nhân viên để giữ chân nhân tài.
- Ứng viên thì cần biết kỹ năng nào đang được trả lương cao, thành phố nào có cơ hội tốt hơn.
Dữ liệu liên quan:
Bộ dữ liệu Human Resources & Job Market Dataset, gồm 12 trường thông tin chính:
job_title, job_type, position_level, city, experience, skills, job_fields, salary, salary_min, salary_max, unit, feedback.
→ Tổng hợp hơn 80.000 dòng dữ liệu, thể hiện thông tin chi tiết về công việc, mức lương, kỹ năng và phản hồi của nhân viên.
Mục tiêu:
·  Phân tích mức lương theo vị trí, kinh nghiệm và địa điểm.
·  Tìm hiểu kỹ năng nào ảnh hưởng mạnh đến mức lương.
·  Đánh giá mức độ hài lòng của nhân viên theo thành phố và lĩnh vực.
·  Từ đó, đưa ra khuyến nghị cho doanh nghiệp và người lao động.

2.2.2 Xác định câu chuyện
Bằng cách đặt câu hỏi, hình thành giả thuyết, tổng hợp đào sâu dữ liệu để tìm câu trả lời:
🔹 Câu hỏi cốt lõi:
Mức lương thay đổi như thế nào theo cấp bậc và kinh nghiệm?
Thành phố nào có mức lương trung bình cao nhất?
Những kỹ năng nào giúp tăng thu nhập?
Nhân viên ở thành phố/nhóm ngành nào hài lòng nhất?
🔹 Giả thuyết ban đầu:
Lương tăng theo cấp bậc và kinh nghiệm.
Các thành phố lớn (TP.HCM, Hà Nội) có lương cao hơn mặt bằng chung.
Kỹ năng thuộc nhóm IT / Data / Management thường có lương cao hơn.
Feedback tích cực xuất hiện nhiều ở ngành có chính sách tốt.
🔹 Mục tiêu cụ thể:
Mô tả: Tình hình lương hiện tại và chênh lệch theo vị trí, khu vực.
Giải thích: Nguyên nhân tạo ra sự khác biệt (do kỹ năng, kinh nghiệm, lĩnh vực).
Dự đoán/Đề xuất: Kỹ năng nên học hoặc thành phố đáng làm việc nhất.
🔹 Hướng phân tích:
Tìm mối tương quan: giữa experience – salary, skills – avg_salary.
Xác định xu hướng: sự thay đổi lương theo position_level.
Rút ra so sánh: giữa các city hoặc job_fields.

2.2.3 Xác định rõ đối tượng
🔹 Ai cần nghe câu chuyện này?
     - Doanh nghiệp / HR: Muốn hiểu xu hướng lương, kỹ năng hot để điều chỉnh chính sách.
     - Ứng viên / người tìm việc: Muốn biết ngành/lĩnh vực nào có lương cao và cần kỹ năng gì.
🔹 Kiến thức nền của họ:
     - Đã quen với khái niệm “thị trường việc làm” và “mức lương trung bình”.
     - Tuy nhiên, chưa có cái nhìn tổng quan dựa trên dữ liệu thực tế → đây là điều dự án cung      cấp.

2.2.4 Xác định câu chuyện chi tiết
🔹 Bối cảnh:
Dựa trên dữ liệu 85.000+ dòng thu thập từ nhiều ngành nghề và thành phố.
Đã làm sạch và chuẩn hóa dữ liệu (đơn vị tiền tệ, nhóm kinh nghiệm, phân loại kỹ năng).
🔹 Cấu trúc câu chuyện:
Mở đầu:
 “Thị trường lao động Việt Nam đang thay đổi ra sao về lương và kỹ năng?”
Thân bài:
Insight 1: So sánh lương trung bình theo position level và experience.
Insight 2: Thành phố nào trả lương cao nhất cho các vị trí hot?
Insight 3: Kỹ năng nào xuất hiện nhiều trong các công việc có lương cao?
Insight 4: Feedback của nhân viên thể hiện điều gì về sự hài lòng?
Kết luận:
Tổng hợp những xu hướng chính.
Đề xuất chiến lược cho HR hoặc người lao động.
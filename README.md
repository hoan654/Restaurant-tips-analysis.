# Restaurant-tips-analysis.
Dự án này phân tích một tập dữ liệu về tiền tip trong nhà hàng nhằm tìm hiểu các yếu tố ảnh hưởng đến mức tip của khách hàng. Phân tích được thực hiện bằng Python trong Jupyter Notebook, bao gồm các kiểm định thống kê, trực quan hóa và rút ra insight phục vụ kinh doanh.

---

## 📊 Mô Tả Dự Án

Mục tiêu của dự án là đánh giá xem các yếu tố như giới tính, tình trạng hút thuốc, ngày trong tuần, hoặc thời điểm dùng bữa (trưa/tối) có ảnh hưởng đến số tiền tip hay không. Qua đó, đưa ra các đề xuất giúp nhà hàng nâng cao chất lượng dịch vụ và doanh thu.

---

## 🗂️ Thông Tin Về Dữ Liệu

- **Nguồn dữ liệu**: [Tips Dataset từ thư viện Seaborn](https://github.com/mwaskom/seaborn-data/blob/master/tips.csv)
- **Mô tả**: Tập dữ liệu bao gồm các cột:
  - `total_bill`, `tip`, `sex`, `smoker`, `day`, `time`, `size`
- **Cách lấy dữ liệu**: Dữ liệu được tải trực tiếp bằng lệnh `sns.load_dataset("tips")`, không cần tải về ngoài.

---

## 🎯 Mục Tiêu Chính

1. Phân tích hành vi tip theo:
   - Giới tính (Nam có tip nhiều hơn không?)
   - Hút thuốc (Người hút thuốc có tip nhiều hơn?)
   - Cuối tuần vs ngày thường (Tip nhiều hơn vào cuối tuần?)
   - Bữa trưa vs bữa tối (Dinner có mang lại nhiều tip hơn?)
2. Thực hiện kiểm định thống kê (Mann-Whitney U test)
3. Trực quan hóa và rút ra đề xuất kinh doanh thực tiễn

---

## 📈 Kết Quả & Insights

### ✅ Giới tính
- Không có sự khác biệt có ý nghĩa thống kê giữa nam và nữ trong hành vi tip.

### ✅ Hút thuốc
- Không có bằng chứng cho thấy người hút thuốc tip nhiều hơn người không hút.

### ✅ Cuối tuần vs ngày thường
- **Cuối tuần** có mức tip cao hơn **có ý nghĩa thống kê** (p ≈ 0.025) → Nên tăng cường phục vụ và khuyến mãi thứ 7, chủ nhật.

### ✅ Dinner vs Lunch
- **Dinner** mang lại nhiều tip hơn Lunch (p ≈ 0.014) → Tập trung upsell và chất lượng phục vụ buổi tối.

---

## 📌 Hướng Dẫn Chạy Dự Án

1. Mở file `.ipynb` trong Jupyter Notebook hoặc Google Colab  
2. Chạy toàn bộ các ô lệnh theo thứ tự  
3. Biểu đồ và p-value sẽ hiển thị trực tiếp

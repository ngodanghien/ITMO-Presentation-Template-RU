# PhD Thesis Presentation template for ITMO University

Đây là mẫu $\LaTeX$ template cho slide trình bày báo cáo LATS. Nó không phải là mẫu chính thức của ITMO University (Hiện tại trường ĐH cũng không yêu cầu và cũng ko có mẫu chính thức). Tuy nhiên việc trình bày báo cáo bằng slide của $\LaTeX$ là rất được hoan nghêng, và template này đã được 02 Tiến sĩ trình bày trong hội đồng báo cáo LATS của khoa điều khiển (tính đến ngày 28.11.2024) với sự đánh giá tốt về cách trình bày.

## How to use

### Online compilation
* Download the `zip` of this repository;
* Upload it to [Overleaf](https://www.overleaf.com/) (tested November 2024).
### Offline compilation
Recommended uses: [TexStudio](https://www.texstudio.org/) and [TexLive](https://tug.org/texlive/)
- Make sure you have `biber` installed
- Change the bibliography engine from `bibtex` to `biber`
##
- Ưu tiên sử dụng `TexStudio` làm môi trường IDE và `Texlive` làm complier cho $\LaTeX$. 
 - Phần in các ấn phẩm đã xuất bản, sử dụng file `*.bib` với `biber` làm trình biên dịch để theo style của GOST-2008. Có thể làm bằng tay nếu ko thích, hoặc số lượng báo chí public quá nhiều`

## Những lưu ý về cách sử dụng
1. Thay đổi các thông tin các nhân của mình trong file `author.tex`
    - Tên người báo cáo; chuyên ngành; giáo hướng dẫn; print báo chí và list hội thảo. lệnh `\insertpagetitle` sẽ in toàn bộ trang title (page đầu tiên)
2. Nếu cần in mục lục (outline) của file thì sử dụng lệnh: `\insertoutline` (mặc định là in ra)
3. Muốn thay đổi nội dung của thanh footline (ở giữa, bên dưới) thì sử dụng lệnh: `\setfootlinetext{nội dung cần hiện thị}`
4. Nhảy nhanh đến list các slides ở footline phía dưới, bên trái `слайды`. Cứ mỗi lần tạo 1 `frame` mới, cần thêm lệnh `\hypertarget{slide\insertframenumber}{}` ngay phía sau để tự động gán link cho `table of slides`. Sau khi nhấn `F11` ở file `PDF` để chuyển sang chế độ báo cáo, nếu cần vào slide nào đó cho nhanh, hãy click vào `слайды` và chọn slide cụ thể có trong list.
5. Một ví dụ về 1 pager trong file `papers.bib`
    ```bib
    @article{Gerasimov2023a,
        author = {Gerasimov, D and Popov, A and Hien, N.D. and Nikiforov, V},
        journal = {IFAC-PapersOnLine},
        issue = {2},
        number = {2},
        pages = {9185--9190}, 
        title = {Adaptive control of LTV systems with uncertain periodic coefficients},
        url = {https://doi.org/10.1016/j.ifacol.2023.10.160},
        volume = {56},
        year = {2023}
    }
    ``` 

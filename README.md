# Thông Tin
Môn: Phát triển phần mềm quản lý <br>
Họ và Tên: Hà Chung Lương <br>
Mã sinh viên: 2221050318 <br>
Lớp: DCCTCT67_04A

# TÌM HIỂU CHI TIẾT ASP.NET MVC

## 1. Tổng quan về ASP.NET MVC

ASP.NET MVC là một framework phát triển web của Microsoft, dựa trên mô hình kiến trúc **MVC (Model – View – Controller)**.  
Mục tiêu của MVC là:
- Tách biệt rõ ràng giữa **giao diện**, **xử lý logic**, và **dữ liệu**
- Giúp code dễ bảo trì, dễ mở rộng
- Phù hợp cho các ứng dụng web lớn

---

## 2. Cấu trúc thư mục của dự án ASP.NET MVC

Khi tạo một project ASP.NET MVC, Visual Studio sẽ sinh ra các thư mục và file chuẩn như sau:

---

### 2.1. Thư mục Controllers

**Controllers** chứa các lớp Controller, đóng vai trò tiếp nhận và xử lý request từ người dùng.

Đặc điểm:
- Mỗi Controller thường tương ứng với một nhóm chức năng
- Tên Controller **bắt buộc kết thúc bằng `Controller`**
- Kế thừa từ lớp `Controller`


[Route("san-pham")]
public class ProductController : Controller
{
    [Route("danh-sach")]
    public IActionResult List()
    {
        return View();
    }
}

namespace MyProject.Controllers
{
    public class HomeController : Controller
    {
    }
}


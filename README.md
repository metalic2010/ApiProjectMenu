# ������ ����������� ��������
�������� ������ �� ������������ ��������, ������ � ����� ��������� ������������� �����.
������ ������� �� 2 �����:
- ���������� (������ �����������)
- ������� (������ � 1 api, ������� ����� ��� ����� �����������)

## ����������
����������:
1. Program - ����������� ����� � ����������� ����� ��� HealthChecks
2. appsettings.json - ����������� ���� � ����������� ����� ��� HealthChecks
## ������
����������:
1. DataBases
* CategoryMenuDB - ������� ��������� ����
-- GetCategoryMenu() - ����� �� ����������� ������� ���������� �� ���������� ����
- MenuDB - ������� ����
-- GetMenu() - ����� �� ����������� ������� ���������� � ����
- ViewListMenu - view (������������ ������������� ����������� ���� ������)
-- GetViewMenu() - ����� ��� join`� ������
2. HealthChecks
* APIHealthChecks
-- CheckHealthAsync() - ��������� ����������� ����������
-- IsDatabaseConnectionOkAsync() - ��������� ������ �� ����������
3. Controllers
* MenuController (3 get �������)
-- GetMenu - api ����� � ������� ���������� � ����
-- GetCategoryMenu - api ����� � ������� ���������� � ���������� ����
-- GetViewMenu - api ����� � ������� ������� ���������� � ����
4. Menu - ����� � ��������� ����, ��������� ���� � view
5. Program - ����������� ����� � ����������� ����� ��� HealthChecks

## ���������� �� ����� � �������
- C# (ASP .NET Core Web API)
-- [AspNetCore.HealthChecks.UI](https://github.com/Xabaril/AspNetCore.Diagnostics.HealthChecks)
-- [AspNetCore.HealthChecks.UI.InMemory.Storage](https://github.com/Xabaril/AspNetCore.Diagnostics.HealthChecks)
-- [AspNetCore.HealthChecks.UI.Client](https://github.com/Xabaril/AspNetCore.Diagnostics.HealthChecks)

OpenEPG
========

Electronic Program Guide (EPG) Generator for Digital Video Broadcasting (DVB). EIT p/f, EIT schedule generation and broadcasting.


#### �������� OpenEPG

����������� ������ 
  * ����� �������� ������
  * ������������� ������ � ����������� �������
  * ����������� ���������� ������ ��� � ISO, ��� � � Unicode
  * �������� ������ �� �������� ������������� ������ (Actual), ��� � �� ��������� (Other)

������������ ������ � ������� EIT (EPG)
  * ������� / ��������� �������
  * ���������� �� ��������� ����
  * ����������� �������� ������� (��������, ��� ��������, ��������, ������)
  * ���������� �����������
  * ���� DVB


������ ���������� �� ����� Perl, ��� ��������� ��� ������������ �� ����� ���������, ������� ������������ Perl.
����� ��� ��������� ������� ��������� ���������� [CherryEPG](http://epg.cherryhill.eu/|CherryEPG)

#### ��������� OpenEPG


#### ������������� ��������� ����� (Windows) 
����� ������� � ������� ������.
  - ��������� [����������� ����](http://a4on.tv/openepg.zip)
  - ����������
  - ��������� ���� ������ � ini ����� 
  - ��������� ������.
**������!**

#### ������������� Perl (Windows ��� Linux) 

���� ������ �������� ���, ��� ������ � ������ ���������������� Perl
�������� ������ ����� ��������� �� �����.
������ ���������� ��������� ������
<code perl>
cpan DBD::Firebird
cpan Digest::CRC
cpan DVB::Epg 


cpan DVB::Carousel
cpan Config::INI::Reader
</code>

#### �������� ���������� INI �����

|��������|�������� �� ���������|��������|
|-|-|-|
|DB_NAME | localhost:a4on_db|���� ������ � epg|
|DB_USER | SYSDBA|������������ ����� ������ Firebird |
|DB_PSWD | masterkey|������ ������������ |
|DAYS    | 7|�� ����� ���������� ���� ����������� EIT|
|TMP     | b:\epg.pl| ��� ������ ��������� �����|
|RELOAD_TIME | 5|����� ������� ����� ������������ �����|
|EXPORT_TS   | 0|�������������� TS � ���� 1. �� ����. = 0|
|NETWORK_ID  | 1|ID ���� � ������� �������� ��������� �� ������ ���� � ��������� ����� ����� � ���� ��|

<code ini>
[EPG]
DB_NAME = localhost:D:/EPG/DB/A4on_db.fdb
DB_USER = SYSDBA
DB_PSWD = masterkey
DAYS    = 7
TMP     = b:\epg.pl
RELOAD_TIME = 5
EXPORT_TS   = 0
NETWORK_ID  = 1
</code>
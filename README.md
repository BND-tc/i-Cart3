# i-Cart3

�I�[�v���\�[�X�ړ����{�b�g�v���b�g�t�H�[��i-Cart3 �̐���ɕK�v�ȏ��̃��|�W�g��

## �p�[�c���X�g (Parts list)
100W/200W���[�^�[�ł̑g���ɕK�v�ȕ��i�\���\�ł�

60W���[�^�[�ł��ߓ����Ɍ��J�\��ł�


## 3D���f���f�[�^ (3D Model Data)
Parasolid�`����STEP�`���̃��f���f�[�^�ł�


## �\�� (Configuraion)
�V�X�e������щ�H�̍\���̎����ł�

iCart3_Configuration.pdf���Q�l�ɔz�������Ă�������

## �\�t�g�E�F�A (Software)
i-Cart3�p�̃\�t�g�E�F�A����ѐݒ�t�@�C���ł�

### yp-spur(BLVR�Ή�)
> https://github.com/BND-tc/yp-spur

��L�r���h�̍ۂɂ�libmodbus���K�v�ƂȂ�܂�

BLVR�ɂ͂��炩���ߍ��E���[�^�[�h���C�o��mxex�ݒ�t�@�C����K�p���Ă�������

### yp-spur�P�̎��s��
> /usr/local/bin/ypspur-coordinator -d PORT_PATH --blvr -p PARAM_PATH

> /usr/local/bin/ypspur-coordinator -d /dev/ttyUSB0 --blvr -p /home/pi/iCart3_200W.param

### ros���s��
> rosrun ypspur_ros ypspur_ros _ypspur_bin:=/usr/local/bin/ypspur-coordinator _port:=[PORT_PATH]--blvr _param_file:=[PARAM_PATH] _compatible:=1

> rosrun ypspur_ros ypspur_ros _ypspur_bin:=/usr/local/bin/ypspur-coordinator _port:=/dev/ttyUSB0--blvr _param_file:=/home/pi/iCart3_200W.param _compatible:=1

<strong> --blvr�I�v�V�����̋L�ڂ��f�o�C�X�|�[�g�̒���ɃX�y�[�X�����ŋL�ڂ��Ă��������B</strong>

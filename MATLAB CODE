clc;
clear all;
close all;
%Reas the input image
k=imread('dsa.jpeg');
[x y z]=size(k);
k=double(k);
for i=1:x
    for j=1:y
        if k(i,j)>=0 & k(i,j)<50
            m(i,j,1)=k(i,j,1)+5;
            m(i,j,2)=k(i,j)+10;
            m(i,j,3)=k(i,j)+10;
        end
        if k(i,j)>=50 & k(i,j)<100
            m(i,j,1)=k(i,j)+35;
            m(i,j,2)=k(i,j)+28;
            m(i,j,3)=k(i,j)+10;
        end
        if k(i,j)>=100 & k(i,j)<150
            m(i,j,1)=k(i,j)+52;
            m(i,j,2)=k(i,j)+30;
            m(i,j,3)=k(i,j)+15;
        end
        if k(i,j)>=150 & k(i,j)<200
            m(i,j,1)=k(i,j)+50;
            m(i,j,2)=k(i,j)+40;
            m(i,j,3)=k(i,j)+25;
        end
        if k(i,j)>=200 & k(i,j)<=256
            m(i,j,1)=k(i,j)+120;
            m(i,j,2)=k(i,j)+60;
            m(i,j,3)=k(i,j)+45;
        end
    end
end
%Plotting of input images.
subplot(2,2,1)
imshow(uint8(k),[]);
title('INPUT DSA IMAGE');
subplot(2,2,2)
imshow(uint8(m),[]);
title('COLOURED DSA IMAGE');
 

%COLOUR CODED DSA IMAGE
x=imread('output_angio.jpeg');
r(:,:,:)=255-x(:,:,:);
subplot(2,2,3)
imshow(r);
title("COLOUR CODED DSA IMAGE");


%ENHANCED DSA IMAGE
x=imread("review2_output.jpeg")
z=0.8*(x-55);
subplot(2,2,4)
imshow(z);
title("ENHANCED DSA IMAGE");

%PLOTTING OF IMAGES SEPERATELY
figure;
imshow(uint8(k),[]);
title('INPUT DSA IMAGE');
figure;
imshow(uint8(m),[]);
title('COLOURED DSA IMAGE');
figure;
imshow(r);
title("IMPROVED DSA IMAGE");
figure;
imshow(z);
title("ENHANCED DSA IMAGE");

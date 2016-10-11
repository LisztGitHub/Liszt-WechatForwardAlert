# Liszt-WechatForwardAlert
  <img src="https://github.com/LisztGitHub/Liszt-WechatForwardAlert/blob/master/Liszt.gif" />
#
    #import <UIKit/UIKit.h>

    typedef NS_ENUM(NSInteger, ContentType){
       /** 图片*/
        Content_Image,
       /** 文字*/
       Content_Text,
        /** Gif*/
        Content_Gif
    };

    /** 点击按钮回调*/
    typedef void (^completionHandlerBlock)(NSInteger buttonClickIndex);

    @interface ForwardAlert : UIView
    /**
    *  初始化Alert
    *  @param title 转发用户名称
    *  @param images 用户头像
    *  @param content 转发内容
    *  @param buttonHandler 点击回调Block
    */
    - (instancetype)initWithTitle:(NSString *)title images:(NSArray *)images content:(id)content contentType:(ContentType)type buttonHandler:(completionHandlerBlock)completionHandler;


    /** 显示*/
    - (void)show;

    @end
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

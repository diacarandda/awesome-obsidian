
 
# How to Use Sip Component V2 9 For Delphi 13 to Make and Answer Phone Calls in Your Applications
  
If you are looking for a way to add voice communication functionality to your Delphi applications, you might want to check out Sip Component V2 9 For Delphi 13. This is a non-visual component that allows you to make and answer phone calls using SIP protocol. You can also play and record audio files, send DTMF codes, and make conference calls with this component.
  
In this article, we will show you how to use Sip Component V2 9 For Delphi 13 to create a simple softphone application that can make and answer phone calls. You will need an account from a SIP provider or a PBX system to use this component.
 
**DOWNLOAD ✦ [https://t.co/NMHVdn9P9k](https://t.co/NMHVdn9P9k)**


  
## Setting Up the Component
  
The first step is to create an instance of the TSipClient component and assign its properties and events. You can either install the component in your Delphi environment and place it on your form, or create it dynamically at runtime. Here is an example of how to create the component at runtime:

    procedure TForm1.FormCreate(Sender: TObject);
    begin
      FSipClient := TSipClient.Create(nil);
      FSipClient.Host := 'sipprovider.com';
      FSipClient.User := 'myusername';
      FSipClient.Password := 'mypassword';
      // Assigning event handler procedures
      FSipCLient.OnRegistration := SipClientRegistration;
      FSipClient.OnCall := SipClientCall;
      FSipClient.OnAnswer := SipClientAnswer;
      FSipCLient.OnBye := SipClientBye;
      FSipCLient.OnPlayed := SipClientPlayed;
      FSipCLient.OnDtmf := SipClientDtmf;
      // Activate the engine
      FSipClient.Active := True;
      // Start registration on SIP server
      FSipClient.Register;
    end;

The Host, User, and Password properties are the credentials of your SIP account. The OnRegistration event is triggered when the registration process is completed. The OnCall event is triggered when an incoming call is received. The OnAnswer event is triggered when an outgoing call is answered. The OnBye event is triggered when a call is ended. The OnPlayed event is triggered when an audio file is played. The OnDtmf event is triggered when a DTMF code is detected.
  
## Making Phone Calls
  
To make a phone call, you need to use the Call method of the TSipClient component. This method takes a string parameter that is the phone number or SIP address of the callee. It returns an ICall interface that represents the call session. You can use this interface to control the call, such as ending it or playing audio files. Here is an example of how to make a phone call:

    procedure TForm1.CallButtonClick(Sender: TObject);
    begin
      FCall := FSipClient.Call('18025551111');
    end;

## Answering Phone Calls
  
To answer an incoming phone call, you need to use the Answer method of the ICall interface that is passed as a parameter in the OnCall event of the TSipClient component. Here is an example of how to answer an incoming phone call:

    procedure TForm1.SipClientCall(Sender: TObject; const ACall: ICall);
    begin
      FCall := ACall;
      FCall.Answer;
    end;

## Ending Phone Calls
  
To end a phone call, you need to use the EndCall method of the ICall interface that represents the call session. You can also use this method to reject an incoming call before answering it. Here is an example of how to end a phone call:

    procedure TForm1.HangupButtonClick(Sender: TObject);
    begin
      FCall.EndCall;
      FCall := nil;
    end;

## Playing and Recording Audio Files
  
You can also use the Sip Component V2 9 For Delphi 13 to play and record audio files during a call session. To
 8cf37b1e13
 
